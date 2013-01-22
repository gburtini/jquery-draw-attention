# jQuery.drawAttention.js

## Instructions
1. call $.drawAttention() to start a highlighting context
2. call $("selector").drawAttention("add"); to add to the highlighted elements
3. call $("selector").drawAttention("remove"); to remove from the highlighted elements
4. call $.drawAttention("destroy"); to destroy the highlighting context and return to the regular page

## Known Issues
* uses z-index to move elements above the shade
* uses pointer-events to allow clicks to pass through the shade (may not be desired and has poor support: http://caniuse.com/pointer-events)
* transparent elements "pull up" their background color above the shade -- this may not be desirable if: 
  * 1. the background color is "close" to the shade color
  * 2. the background is actually an image (may just be lost).
* - transparency is detected with rgba(0, 0, 0, 0) which is probably not the ideal way to do it. 

## License - you must retain this notice in ALL redistributions

Copyright 2013 Giuseppe Burtini      https://github.com/gburtini

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this library except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
