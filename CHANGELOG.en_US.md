## 2.2.0 (2021-04-06)

### โจ Features

- Added `headerTitle` slot
- New printing example
- Added about interface

### โจ Refactor

- Remove useFullScreen function
- tinymce changed from Cdn to npm (the package size is too large)
- Dashboard refactoring
- Remove ApexCharts and examples

### ๐ Bug Fixes

- Make sure the breadcrumbs are displayed correctly
- Fixed the issue of tinymce upload button disappearing in full screen mode
- Make sure that the title changes normally after logging in again
- Ensure that the background mode login is normal
- Fix TableAction click event issue

## 2.1.1 (2021-03-26)

### โจ Features

- Added hideChildrenInMenu configuration for routing. Used to hide submenu
- Built-in expand/collapse all functions in the tree form

### โจ Refactor

- Refactor the routing multi-layer mode to solve the problem of multiple implementations of nested keepalives

### ๐ Bug Fixes

- Ensure that the CountDownInput component is reset to the empty value
- Fix the display problem on the small screen in split mode
- Fix table height calculation problem
- Fix the problem that components cannot be obtained by background routing
- Fix Modal component loadingTip configuration does not take effect
- Fix the background permission command does not take effect
- Make sure the progress bar is closed properly
- Fix the problem of invalid table check column configuration
- Ensure that the first level menu can be hidden
- Ensure that the hidden fields of the form are verified properly

### ๐ซ Chores

- Remove ls-lint

### ๐ซ Chores

- ็งป้ค ls-lint

## 2.1.0 (2021-03-15)

### โจ Features

- Added svg mode to icon selector
- Added time component
- Added AutoNavi/Baidu/Google Map example

### โจ Refactor

- Refactor the project to solve the hot update problem caused by circular dependencies
- Remove vueHelper/useClickoutside, use @vueuse/core instead

### ๐ Bug Fixes

- Ensure that the value of `table action` is updated correctly
- Fix the animation of page switching cannot be closed
- Fix `PageWrapper`title not showing
- Fix the known issues of the table
- Fix the problem that the BasicTree component can't customize the title
- Fix the button style problem after theme switching

## 2.0.3 (2021-03-07)

### โจ Features

- `BasicTree` added `clickRowToExpand`, used to click tree node to expand
- Added SvgIcon plugin and examples
- Add the department tree on the left side of the account management interfaceยท

### โก Performance Improvements

- Pagination parameters are no longer carried when the table is closed
- The login page monitors the carriage return event to log in
- When the adaptive size of the table is set, the height is filled according to the screen.
- Tree scroll bar optimization
- Optimize the loading speed of local development

### ๐ Bug Fixes

- Fix known issues with `Description`
- Fix known issues with `BasicForm`
- Fix the logic problem of show attribute of ActionItem under `BasicTree`
- Fix the style error of the tree component demo example
- Repair account management to add new but not cleared old data
- The form component should allow the setFieldsValue method to be null or undefined
- Ensure that the single-level breadcrumbs jump correctly
- Ensure that the Form component does not verify hidden form items

## 2.0.2 (2021-03-04)

### โจ Refactor

- Refactored multi-language modules to support lazy loading and remote loading

### โจ Features

- axios supports form-data format request
- Added icon selector component (support local and online methods)
- Added WebSocket examples and service scripts
- Added the `renderIcon` property to the Tree component to control the display of level icons
- Tree->actionItem added show attribute, used to dynamically control button display
- New toolbar/title/search function for Tree
- Added department management/password modification/account management/role management/menu management sample interface

### โก Performance Improvements

- Optimized login interface animation
- Fix the problem of excessively large github warehouse.
- Hide table full screen button by default
- `crypto-es` is changed to `crypto-js` to reduce the package size
- `types` directory moved to the root directory, compatible with other directory global types

### ๐ Bug Fixes

- Fix the warning problem of verification code component
- Fix the table cannot get the selected row correctly
- Fixed modal height calculation error in full screen state
- Fix some table style issues
- Fix the invalidation of the tree form `indentSize` setting

## 2.0.1 (2021-02-21)

### โจ Refactor

- Refactored login page, new registration page/reset password page/mobile phone login/QR code login

### โจ Features

- Added the `settingButtonPosition` configuration item for configuring the position of the `settings` button
- `modal` can switch the full screen by double-clicking the head
- Added `CountDownInput` component

### โก Performance Improvements

- Optimize the editable center style and the width of the drop-down box is too short
- The `edit-change` event listener when the table is added and edited

### ๐ Bug Fixes

- Fix image preview style error
- Fix icon style problem
- Fix the drop-down echo problem of editable table

## 2.0.0 (2021-02-18)

## Breaking changes

- `echarts` is upgraded to 5.0 and introduced on demand (just use `useECharts`).

### โจ Refactor

- Removed `global.less`, `mixin.less`, `design/helper`, replaced by `windicss`, and need to modify the corresponding styles if they are useful

### โจ Features

- useModal adds the return value function `redoModalHeight`, which is used to refresh the modal height when the modal is dynamic content
- Upgrade husky to 5.0
- Added `brotli`|`gzip` compression and related test commands
- Re-introduction of `windicss` (same as `tailwind`). Faster in speed

### โก Performance Improvements

- Adjust the return value of the interface to obtain user information in array format
- Fix the error-log list as the system route

### ๐ Bug Fixes

- Fix the issue of upload component maxNumber invalid
- Fix package sourcemap error report
- Fix code debugger location display error
- Fix the issue of mock plugin post request error
- Fix some themes color value error
- Fix the table in editable row status and press Enter to confirm

### ๐ซ Chores

- Documentation update
- Upgrade ant-design-vue to `2.0.0`
- Upgrade vite to `2.0.0`

## 2.0.0-rc.18 (2021-02-05)

### โจ Features

- `ApiSelect` adds `numberToString` property, which is used to convert all the value of `number` into `string`
- Added theme color switch
- Packed image compression

### โก Performance Improvements

When mock is not used, move `mock.js` out of the package file

### ๐ Bug Fixes

- Fix modal height calculation error
- Fix the pop-up menu when the menu is clicked on the tab when the menu is collapsed
- Fix the problem that the initial value of form is 0
- Fix table wrapping problem
- Fix the menu outside link does not jump
- Fix the display problem at the top of the menu
- Fix the issue of `modifyVars` configuration failure

## 2.0.0-rc.17 (2020-01-18)

### โจ Refactor

- Added `SimpleMenu` component to replace the left menu component (the top menu is not replaced, the function should be as simple as possible without stuck). Solve the menu stuck problem.
- The `ant-design-vue` component is no longer registered globally. In order to better coordinate with the introduction of css on demand. If you need to register globally, you need to add it yourself

### โจ Features

- `css` import on demand

### ๐ Bug Fixes

- Fix `TableAction` icon problem
- Fix the problem of missing menu folding buttons
- Fix menu related issues
- Fix moment multilingual issue

## 2.0.0-rc.16 (2020-01-12)

### โจ Refactor

- Independent component configuration to `/@/settings/componentsSetting`
- `colorSetting` and `designSetting` are now merged into `designSetting`
- `ant-design-vue` component registration moved to `components/registerComponent`
- Remove the `setup` folder
- Upgrade to `vite2`
- Image preview is changed to `Image` component implementation, temporarily removing functional usage

### โจ Features

- Added `mixSideTrigger` configuration. Used to configure how to open the mixed mode menu on the left. Optional `hover`, default `click`
- Added `mixSideFixed` configuration. Used to fix the left mixed mode menu
- Added `height` and `min-height` properties to the modal component
- Added `PageWrapper` component. And applied to the sample page
- Added tab folding function
- Compatible with older browsers
- tinymce new image upload

### ๐ Bug Fixes

- Fix known issues with table column configuration
- Restore the `isTreeTable` property of the table
- Fix table memory overflow problem
- Fix the function of `layout` shrinking and expanding in split mode
- Fix modal height calculation error
- Fix file upload error

## 2.0.0-rc.15 (2020-12-31)

### โจ Table destructive update

- Refactored editable cells and editable rows. See examples for details. The writing has changed. For editable tables.

- Form editing supports form validation

- Added the following configuration in the table column configuration

```bash
{

  # Whether to display columns by default. Those that are not displayed can be opened in the column configuration
  defaultHidden?: boolean;
  # Help text on the right side of the column header
  helpMessage?: string | string[];
  # Custom formatting Cell content. Support time/enumeration automatic conversion
  format?: CellFormat;

  # Editable
  # Is it an editable cell
  edit?: boolean;
  # Is it an editable line
  editRow?: boolean;
  # Edit status.
  editable?: boolean;
  # Edit component
  editComponent?: ComponentType;
  # The parameters of the corresponding component
  editComponentProps?: Recordable;
  # Check
  editRule?: boolean | ((text: string, record: Recordable) => Promise<string>);
  # Value enumeration conversion
  editValueMap?: (value: any) => string;
  # Trigger editing Zhenghang
  record.onEditRow?: () => void;
}

```

### โจ Table reconstruction

- Added `clickToRowSelect` attribute. Used to control whether the clicked row is checked or not
- Monitor row click event
- Add column drag and drop and column fix function for the table column configuration button.
- Added `defaultHidden` attribute to table column configuration. Used to hide by default. You can configure the tick display in the table column
- More powerful column configuration
- useTable: Support for dynamically changing parameters. You can pass in `Ref` type and `Computed` type for dynamic changes
- useTable: Added return function `getForm`. Can be used to manipulate forms in the form Fix known issues in the table

### โจ Features

- Added `v-ripple` water ripple command
- Added the left menu mixed mode
- Add an example of markdown embedded in the form
- Add an example of a page outside the main frame
- `route.meta` added `currentActiveMenu`, `hideTab`, and `hideMenu` parameters to control the display and hide of the crumb-level menu on the detail page.
- Added breadcrumb navigation example
- form: Added `suffix` attribute to configure suffix content
- form: Added remote drop-down `ApiSelect` and examples
- form: Add `autoFocusFirstItem` configuration. Used to configure whether to focus on the first input box of the form
- useForm: Support for dynamically changing parameters. You can pass in `Ref` type and `Computed` type for dynamic changes

### โก Performance Improvements

- Optimize the scroll bar components of `modal` and `drawer`
- table: remove the `isTreeTable` attribute
- Import `less` files globally. No need to manually re-introduce the component

### ๐ซ Chores

- Upgrade `ant-design-vue` to `2.0.0-rc.7`
- Upgrade `vue` to `3.0.5`

### ๐ Bug Fixes

- Fixed the issue of missing scroll bars in mixed mode
- Fix the invalid configuration of environment variables and the logo address problem in history mode
- Fix the calculation error of width and height caused by switching page of chart library
- Fixed the issue of multi-language configuration `Locale.show` causing the configuration not to take effect
- Fix routing type error
- Fix the problem of invalid permissions when the menu is split
- Iframe loads early when closing multi-tab pages
- Fix known issues with `modal` and `drawer`
- Fix the problem of mixing mode adaptation in the left menu

## 2.0.0-rc.14 (2020-12-15)

### โจ Features

-Remove the left menu search, add the top menu search function -Layout mobile terminal adaptation. Business page is not adapted -axios join the joinTime configuration. Control whether the response includes a timestamp

### โก Performance Improvements

-Import components asynchronously -Optimize the overall structure -Replace the default scroll bar of the menu as a scroll component -Menu performance optimization

### ๐ซ Chores

-Return to the top to adjust the style to avoid covering other elements -Upgrade `ant-design-vue` to `2.0.0-rc.5` -Refresh button layout adjustment -`route.meta` removes the `externalLink` attribute

### โจ Refactor

-`openModal` and `openDrawer` third parameter `openOnSet` is set to true by default

### ๐ Bug Fixes

-Fixed an issue where multi-level routing cache caused components to render multiple times -Fixed the problem of disappearing after switching the map chart -Fix the issue of successful login and notify disappearing -Modify the names of `VirtualScroll` and `ImportExcel` components as `VScroll` and `ImpExcel` to temporarily solve the memory overflow of components containing keywords in the vue template -Fix axios case problem -Fix button style problem -Fix the problem of menu split mode -Fix the issue of invalid data transmission when using emits in `Modal` and `Drawer` components -Fix the known problems of the menu -Fix the issue of upload component api failure -Fix the problem of invalid menu permission filtering

## 2.0.0-rc.13 (2020-12-10)

## (Breaking changes) Breaking changes

-Route reconstruction, the previous format is no longer supported. Change to support the original default structure of vue-router, the specific format can be changed by referring to the example. Realize multi-level route caching, and no longer convert routes to level 2. -Refactor breadcrumbs and use antd's breadcrumbs component. The previous component has been deleted

### โจ Features

-Restore the default loading of antdv, refactor the `Loading` component, and add `useLoading` and `v-loading` instructions. And add examples -i18n supports vscode `i18n-ally` plugin -New examples of increased routing cache -Packaged code split (experimental) -Extract upload address to global variable, package can be dynamically configured

### โจ Refactor

-Tree component ref function call to delete `$` -Reconstruction and beautification of the lock screen interface, delete unnecessary background pictures

### โก Performance Improvements

-Page switching loading logic modification. Regardless of whether the loaded page is closed or not, loading will not be displayed when opened again (pages that have been opened are opened again faster, and loading is not required, and the logic of the top progress bar is the same), and it will be restored after refreshing.

### ๐ซ Chores

-First screen loading modification -Upgrade `vue` to `3.0.4` -Upgrade `ant-design-vue` to `2.0.0-rc.3` -Re-introduction of `vueuse` -Remove the `afterCloseLoading` attribute in route meta -Documentation update

### ๐ Bug Fixes

-Fix form i18n error -Fix the inconsistent size of menu icons -Fix the calculation of the top menu width -Fix table tabSetting problem -Repair file upload and delete invalidation -Fix the problem of editing and saving table rows

## 2.0.0-rc.12 (2020-11-30)

## (็?ดๅๆงๆดๆฐ) Breaking changes

- The ClickOutSide component import method is changed from `import ClickOutSide from'/@/components/ClickOutSide/index.vue'` to `import {ClickOutSide} from'/@/components/ClickOutSide'`
- Button component import method changed from `import Button from'/@/components/Button/index.vue'` to `import {Button} from'/@/components/Button'`
- StrengthMeter component import method is changed from `import StrengthMeter from'/@/components/StrengthMeter'` to `import {StrengthMeter} from'/@/components/StrengthMeter'`
- In addition to the examples, the global internationalization function is added, supporting Chinese and English

### โจ Refactor

- Refactor the overall layout. Change the code implementation method. Code is more streamlined
- Configuration item reconstruction
- Remove messageSetting configuration
- BasicTitle component `showSpan`=> `span`

### โจ Features

- The cache can be configured to encrypt or not, and Aes encryption is enabled in the production environment by default
- Add tab drag and drop sort
- Added LayoutFooter. The default display, can be closed in the configuration

### โก Performance Improvements

- Optimized the problem that the full screen animation of `Modal` component is not smooth

### ๐ Bug Fixes

- tree: Fix the problem that the text exceeds the operation button
- useRedo: Fix the problem of missing parameters when refreshing the page through useRedo
- form: Fix the problem that the form verification is first set in the verification and the console error message
- `modal`&`drawer` fix the problem of component passing array parameters
- form: fix `updateSchema` does not take effect when the value contains `[]`
- table: Fix the display problem of the table `TableAction` icon
- table: fix table column settings not displayed by `setColumns` setting

### ๐ซ Chores

- Update antdv to `2.0.0-rc.2`
- Update vue to `3.0.3`
- Update vite to `1.0.0.rc13`
- Temporarily delete `@vueuse/core`. After it is stable, it will be integrated. It is currently not stable.

## 2.0.0-rc.11 (2020-11-18)

### โจ Features

- Added base64 file stream download
- Optimize upload components and examples
- New editable row example
- Add a personal page
- New form page
- Add details page
- Integrate upload components into form by default

### ๐ซ Chores

- Update antdv to `2.0.0-rc.1` (temporarily restore to beta15, rc1 menu freezes too seriously.)
- Add some notes

### โจ Refactor

- Removed `receiveDrawerDataRef` and `transferDrawerData` properties of `useModal` and `useDrawer`
- `openModal` and `openDrawer` corresponding to `useModal` and `useDrawer` extend the third parameter. Used to open the trigger callback again

### ๐ Bug Fixes

- Repair form inputNumber verification error
- Fix the error of setting the default value of the form
- Fix the problem of occupying position when the menu collapse button is hidden
- Fix the form baseColProps does not take effect

## 2.0.0-rc.10 (2020-11-13)

### โจ Refactor

- Refactor hook, introduce `@vueuse`, delete existing `hook`, optimize existing hook
- สปUseEvent` renamed ->สปuseEventListener`
- Delete the four types `SelectOptGroup`, `SelectOption`, `Transfer`, and `Radio` from the form `ComponentType`. Modify the `RadioButtonGroup` component

### โจ Features

- `componentsProps` support function type of form item
- Added tag display to the menu, supporting 4 types of colors and dot display
- New menu and top bar color selection color matching
- Add sample result page
- New file download example

### โก Wip

- Upload components (not completed, testing...)

### โก Performance Improvements

- Optimize settingDrawer code
- Optimize the switching speed of multiple tabs
- Add form customization and dynamic capabilities

### ๐ Bug Fixes

- Fixed multiple rich text editors showing only one
- Fixed the problem of not redirecting to the original page after logging in again after expiration
- Fix window system dynamic introduction error
- Fix page type error
- Fixed an error when the form switch and checkBox were used separately

## 2.0.0-rc.9 (2020-11-9)

### โจ Features

- Menu trigger can select location
- Add an example of rich text embedded form
- Added `required` attribute to form component schema. Simplified configuration
- The second parameter of openModal and openDrawer can be passed internally instead of `transferModalData`
- Routes with parameters can be cached

### โจ Refactor

- Refactored the logic of the menu generated by the background
- Route Module structural transformation

### โก Performance Improvements

- Menu performance continues to be optimized and smoother
- Optimize lazy loading components and examples
- layout style fine-tuning

### ๐ซ Chores

- Delete menu background image
- Update the version of สปant-design-vue`to`beta15`
- Update `vite` version to `rc.9`
- Exception page adjustment
- `BasicTitle` Color blocks are not displayed by default

### ๐ Bug Fixes

- Fix table type problem after upgrade
- Fix the problem that the last submenu continues to be displayed when the menu is divided and there is no data in the left menu
- Fix the issue of สปuseMessage` type
- Fix the problem that the form item setting `disabled` does not take effect
- Fix that สปuseECharts`can't adapt when`resize`, and an error is reported
- Fix that `resize` is not deleted after สปuseWatermark` is cleared
- Fix form verification problem
- Fixed the problem that the multi-level header configuration does not take effect

## 2.0.0-rc.8 (2020-11-2)

### โจ Features

- Global loading add text
- Right-click menu supports multiple levels

### ๐ซ Chores

- Login cache changed from sessionStorage to LocalStorage

### โก Performance Improvements

- Update สปant-design-vue`to`beta.12`
- Layout interface layout style adjustment
- Optimize lazy loading components
- Optimize table rendering performance
- Add animation to form folding search icon
- routeModule can ignore the layout configuration. Convenient to configure the first-level menu

### ๐ Bug Fixes

- Fix table type error
- Fix bug in mock paging tool
- Fix the folding problem of the search form when the table is opened
- Fix the problem of fixed column style when the table size is samll
- Fixed the error report when closing multiple tabs
- Fix message type error

## 2.0.0-rc.7 (2020-10-31)

### โจ Features

- The form component now supports directly passing in the model to directly perform the set operation, please refer to **Component -> Popup Extension -> Open Popup and Pass Data**

- The useModalInner of modal now supports the incoming callback function to receive the value passed in from the external `transferModalData`

  - Used to handle the setting values โโof components such as forms when the pop-up window is opened. Refer to **Component -> Popup Extension -> Open Popup and Pass Data**
  - The value of `receiveModalDataRef` is temporarily reserved. Use as little as possible. It may be deleted later.

- The drawerโs useDrawerInner now supports the incoming callback function to receive the value passed in from the external `transferModalData`,๏ผ
  - Used to handle the setting values โโof components such as forms for opening the drawer Refer to **Component->Drawer Extension->Open the drawer and transfer data**
  - The value of `receiveModalDataRef` is temporarily reserved. Use as little as possible. It may be deleted later.

### โจ Refactor

- Form code optimization and reconstruction

### โก Performance Improvements

- Modal slot can be overwritten
- Optimize table embedding height calculation problem

### ๐ซ Chores

- Add some notes
- pwa icon supplement
- Type adjustment
- Upgrade สปant-design-vue`to`beta.11`, and modify the known issues brought about, and some issues will be resolved after discovery

### ๐ Bug Fixes

- Fix the timeout error of local proxy post interface to https address
- Fix modal full screen height calculation problem when footer is not displayed
- Fix the error that the verification information is not deleted when the form is reset
- Fix the style problem of the split mode of the top menu
- Fix the invalidation of table expansion icon animation

## 2.0.0-rc.6 (2020-10-28)

### โจ Features

- Added `pwa` function, which can be turned on in `.env.production`
- Button component extends `preIcon` and `postIcon` attributes to add icons before and after the text
- Restore the breadcrumb display icon function

### ๐ซ Chores

- Upgrade vite version to `v1.0.0.rc8`
- vite.config.ts internal plugins extraction
- Build directory structure adjustment
- Dependency update
- Documentation update
- Modify the default route switching animation

### โก Performance Improvements

- `setTitle` logic adjustment
- The sessionStorage and LocalStorage cache settings used by the system expire in `7` days by default

### โจ Refactor

- Separate `vite-plugin-html` and modify the logic of inserting html

### ๐ Bug Fixes

- Fix the warning problem of multiple registration components during hot update
- Fix the login tab page appears after login
- Fix the problem of routing switch parameter disappearance
- Fix the useMessage icon style problem

## # 2.0.0-rc.5 (2020-10-26)

### โจ Features

- Update component documentation
- Breadcrumbs support display icon
- Added tinymce rich text component
- Add submitOnReset to the form to control whether to re-initiate the request when reset
- Added `sortFn` to the table to support custom sorting
- Added animation components and examples
- Added lazy loading/delay loading components and examples

### โจ Refactor

- The detailType of the Drawer component is changed to isDetail

### ๐ซ Chores

- Remove the optional chain syntax in the code
- Form reset logic modification
- Turn off multi-tab page tabs animation
- Upgrade vite version to `v1.0.0.rc6`
- Delete Chinese path warning. rc6 has been fixed

### ๐ Bug Fixes

- Fix the automatic height and display footer display problems of drawer components
- Reset to default value after repairing form query
- Fix the problem of displaying the collapsed menu when there are no child nodes
- Fix the problem of breadcrumb display style
- Fixed the problem of multiple open drag and drop failure when destroyOnClose=true in modal
- Fixed multiple action columns in the table

# 2.0.0-rc.4 (2020-10-21)

### โจ Features

- New configuration toolbar for tables
- New message notification module

### ๐ซ Chores

- The table does not show borders by default
- Dependency update
- Update vue to `v3.0.2`
- Interface style fine-tuning

### โก Performance Improvements

- Optimize the size of the first screen
- Optimize the TableAction component
- Reduce the folding width of the menu

### ๐ Bug Fixes

- Fix the problem of the menu name when the first level menu is folded
- Fix the problem that the preview command is not packaged
- Fix the problem that the form actionColOptions parameter does not take effect
- Fix the problem that the loading does not take effect when refreshing the form

# 2.0.0-rc.3 (2020-10-19)

### โจ Features

- Added excel component and excel/xml/csv/html export example
- Added excel import example
- Added global error handling
- Added markdown components and examples
- The menu name can be displayed when adding a new folding menu

### Docs

- add project doc

### ๐ซ Chores

- update deps

### ๐ Bug Fixes

- Fix the adaptive problem of the top menu
- Fix window system packaging error

# 2.0.0-rc.2 (2020-10-17)

### โจ Features

- Package can be configured to output `gizp`
- Package can be configured to delete `console`
- Routes and menus do not need to be imported manually, they are imported automatically

### ๐ซ Chores

- Upgrade vue to `3.0.1`
- Change `vite` version to daily build version

### ๐ Bug Fixes

- Fix menu error
- Fix the problem of table adaptive height
- Fix the issue of error reporting when executing script in `window system`
- Fix the problem of folding components

### โก Performance Improvements

- Remove menu to minimize background
- Prevent page refresh and re-render menu
- Some other details are optimized

# 2.0.0-rc.1 (2020-10-14)

### โจ Features

- Add a tab with parameters

### โก Performance Improvements

- Optimized menu folding
- Page details optimization
- Compress html after packaging
- Functional reconstruction of preview components and right-click menu
- The preview component operation column is centered

### ๐ซ Chores

- update deps
- Added `README.en-US.md`
- Added `CHANGELOG.en-US.md`

### ๐ Bug Fixes

- Fix page refresh and jump to landing page

# 2.0.0-beta.7 (2020-10-12)

### โก Performance Improvements

- The existing tab switching no longer displays animation and progress bar

### โจ Features

- Added `CountTo` component and sample demo
- Added `closeMessageOnSwitch` and `removeAllHttpPending` to the project configuration file
- The production environment has a separate configuration file for dynamic configuration project configuration
- Added สปuseEcharts` and สปuseApexChart` to facilitate the use of charts, and added related demos
- New workbench interface
- New analysis page interface

### ๐ซ Chores

- Update dependencies

### ๐ Bug Fixes

- Fix routing switch, tab inactive problem

# 2.0.0-beta.6 (2020-10-11)

### ๐ Styles

- Menu style adjustment

### ๐ Bug Fixes

- Fix the problem that editable forms cannot be entered
- Repair packaging errors, no proxy is required in the production environment

### โก Performance Improvements

- Optimize the switching speed of multi-tab pages
- First screen loading animation

# 2.0.0-beta.5 (2020-10-10)

### โป Code Refactoring

- Delete `tailwind css`

### โก Performance Improvements

- Optimize page switching speed

### ๐ซ Chores

- Add `.vscode` and `.github` configuration
- Change menu icon
- Added `.env` configuration file
- Update readme.md

### ๐ Bug Fixes

- Fix the failure of `Tree` component check event

# 2.0.0-beta.4 (2020-10-08)

### ๐ซ Chores

- Remove redundant dependencies

### ๐ Bug Fixes

- Fix page refresh blank
- Fix the invalid table style in the production environment

# 2.0.0-beta.3 (2020-10-07)

### โจ Features

- Added สปopenNProgress` to the project configuration file to control whether to open the top control bar
- Add `Table` component and demo

### ๐ซ Chores

- Add ` github workflows`

# 2.0.0-beta.2 (2020-10-07)

### โจ Features

- Added image preview component

### ๐ง Continuous Integration

- Add githubAction script

# 2.0.0-beta.1(2020-09-30)

### ๐ซ Chores

- Migrate some code from 1.0
- Add README.md description file

### ๐ Bug Fixes

- Fix the problem of form, animation and packaging failure
