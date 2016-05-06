# Country Picker for Android

CountryPicker is a simple library that can be show a country picker. See the example to see more detail.

<img src="https://raw.githubusercontent.com/mukeshsolanki/country-picker/master/Screenshot_20160506-152951.png" width="480" height="800" />

## How to use

Integrating the project is simple a refined all you need to do is add this to your app level gradle file

```java
compile 'com.mukesh:countrypicker:0.0.2'
```

Once the project has been added to gradle the user can implement this with easy.

```java
CountryPicker picker = CountryPicker.newInstance("Select Country");
picker.show(getSupportFragmentManager(), "COUNTRY_PICKER");
picker.setListener(new CountryPickerListener() {
    @Override
    public void onSelectCountry(String name, String code, String dialCode, int flagDrawableResID) {
        // Implement your code here
    }
});
```

That's it your all done.
