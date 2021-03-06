# SearchView

**Note: Version 1.6 is not compatible with 1.5. And Toolbar version is not done yet.**

Persistent SearchView Library with history in Material Design. 
It supports layout like section My apps in Google Play Store.
https://www.google.com/design/spec/patterns/search.html. 

Material colors in the project:
https://gist.github.com/lapism/3b417142300d9dbde3b4

Sample application on:

<a href="https://play.google.com/store/apps/details?id=com.lapism.searchview.sample">
  <img alt="Get it on Google Play"
       src="https://github.com/lapism/SearchView/blob/master/images/google_play.png" />
</a>

# Usage
**Add the dependencies to your gradle file:**
```javascript
dependencies {
        compile 'com.lapism:searchview:1.5' ( 1.6 will be soon )
        }
```

![Screenshot 1]
(https://github.com/lapism/SearchView/blob/master/images/image_1.png)

**In code (Check the Sample project!):**

    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        switch (item.getItemId()) {
            case R.id.action_search: {
                mSearchView.showSearch();
                return true;
            }
            default:
                return super.onOptionsItemSelected(item);
        }
    }

**In xml (Check the Sample project!):**
```xml
<com.lapism.searchview.SearchView
    android:id="@+id/search_view"
    android:layout_width="match_parent"
    android:layout_height="match_parent" />
        
You can find examples of layouts in the Sample project !!!     
```

**Styling SearchView:**
```
1.5
app:search_style = "classic / color"
app:search_version = "light / dark"
app:search_divider = "true / false"
1.6
app:search_version = "toolbar / menu_item"
app:search_hint = "Hint text"
app:search_hint_size = "16sp"
app:search_voice = "true / false"
app:search_voice_text = "Voice text"
app:search_animation_duration = "360"

```

