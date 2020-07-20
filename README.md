# Zoom Recyler Layout

[![platform](https://img.shields.io/badge/platform-Android-yellow.svg)](https://www.android.com)
[![API](https://img.shields.io/badge/API-11%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=22)
[![GitHub license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

An beautiful Zoom Animation Library for RecyclerView Items in Android using Kotlin. 

## Preview
![gif](https://github.com/Spikeysanju/ZoomRecylerLayout/blob/master/horizontal_scroll.gif)

<table style="width:100%">
  <tr>
    <th>1. Horizontal Scroll </th>
    <th>2. Vertical Scroll</th> 
  </tr>
  <tr>
    <td><img src = "https://github.com/Spikeysanju/ZoomRecylerLayout/blob/master/horizontal_scroll.gif"/></td> 
    <td><img src = "https://github.com/Spikeysanju/ZoomRecylerLayout/blob/master/vertical_scroll.gif"/></td> 
   
  </tr>
</table>

## About

An beautiful Zoom Animation for RecyclerView Items in Android using Kotlin. 

## Dependency

Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:



```
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}

```

## Dependency

Add dependency in your app module

```
	dependencies {
	        implementation 'com.github.Spikeysanju:ZoomRecylerLayout:1.0'
	}

```

## Usage

### Kotlin
```
        val linearLayoutManager = ZoomRecyclerLayout(this)
```

### Detailed Usage
```

        val linearLayoutManager = ZoomRecyclerLayout(this)
        linearLayoutManager.orientation = LinearLayoutManager.HORIZONTAL
        linearLayoutManager.reverseLayout = true
        linearLayoutManager.stackFromEnd = true
        recyclerView.layoutManager = linearLayoutManager // Add your recycler view to this ZoomRecycler layout
```
### Orientation Types
```

        linearLayoutManager.orientation = LinearLayoutManager.HORIZONTAL
        linearLayoutManager.orientation = LinearLayoutManager.VERTICAL

        
```

### Use SnapHelper for Auto Center Views
```
        val snapHelper = LinearSnapHelper()
        snapHelper.attachToRecyclerView(recyclerView) // Add your recycler view here
        recyclerView.isNestedScrollingEnabled = false
```

# Donation
If this project help you reduce time to develop, you can give me a cup of coffee :) 

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/paypalme2/spikeysanju)



## License
```


    Copyright 2020 Spikey sanju

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

```
