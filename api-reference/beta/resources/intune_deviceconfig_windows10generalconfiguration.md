﻿# windows10GeneralConfiguration resource type

> **Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

This topic provides descriptions of the declared methods, properties and relationships exposed by the windows10GeneralConfiguration resource.

Inherits from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windows10GeneralConfigurations](../api/intune_deviceconfig_windows10generalconfiguration_list.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) collection|List properties and relationships of the [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) objects.|
|[Get windows10GeneralConfiguration](../api/intune_deviceconfig_windows10generalconfiguration_get.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md)|Read properties and relationships of the [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.|
|[Create windows10GeneralConfiguration](../api/intune_deviceconfig_windows10generalconfiguration_create.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md)|Create a new [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.|
|[Delete windows10GeneralConfiguration](../api/intune_deviceconfig_windows10generalconfiguration_delete.md)|None|Deletes a [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md).|
|[Update windows10GeneralConfiguration](../api/intune_deviceconfig_windows10generalconfiguration_update.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md)|Update the properties of a [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|enableAutomaticRedeployment|Boolean|Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.|
|assignedAccessSingleModeUserName|String|This policy setting allows to define the user account that will be locked to Single App Kiosk Mode.|
|assignedAccessSingleModeAppUserModelId|String|This policy setting allows to define the Application User Model ID (AUMID) that will be locked to Single App Kiosk Mode.|
|microsoftAccountSignInAssistantSettings|[signInAssistantOptions](../resources/intune_deviceconfig_signinassistantoptions.md)|Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service. Possible values are: `notConfigured`, `disabled`.|
|authenticationAllowSecondaryDevice|Boolean|Allows secondary authentication devices to work with Windows.|
|authenticationAllowFIDODevice|Boolean|Indicates whether or not to allow authentication using FIDO device (https://fidoalliance.org/)|
|cryptographyAllowFipsAlgorithmPolicy|Boolean|Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.|
|displayAppListWithGdiDPIScalingTurnedOn|String collection|List of legacy applications that have GDI DPI Scaling turned on.|
|displayAppListWithGdiDPIScalingTurnedOff|String collection|List of legacy applications that have GDI DPI Scaling turned off.|
|enterpriseCloudPrintDiscoveryEndPoint|String|Endpoint for discovering cloud printers.|
|enterpriseCloudPrintOAuthAuthority|String|Authentication endpoint for acquiring OAuth tokens.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.|
|enterpriseCloudPrintResourceIdentifier|String|OAuth resource URI for print service as configured in the Azure portal.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Maximum number of printers that should be queried from a discovery endpoint. This is a mobile only setting. Valid values 1 to 65535|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|OAuth resource URI for printer discovery service as configured in Azure portal.|
|messagingBlockSync|Boolean|Indicates whether or not to block text message back up and restore and Messaging Everywhere.|
|messagingBlockMMS|Boolean|Indicates whether or not to block the the MMS send/receive functionality on the device.|
|messagingBlockRichCommunicationServices|Boolean|Indicates whether or not to block the the RCS send/receive functionality on the device.|
|printerNames|String collection|Automatically provision printers based on their names (network host names).|
|printerDefaultName|String|Name (network host name) of an installed printer.|
|printerBlockAddition|Boolean|Prevent user installation of additional printers from printers settings.|
|searchBlockDiacritics|Boolean|Specifies if search can use diacritics.|
|searchDisableAutoLanguageDetection|Boolean|Specifies whether to use automatic language detection when indexing content and properties.|
|searchDisableIndexingEncryptedItems|Boolean|Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.|
|searchEnableRemoteQueries|Boolean|Indicates whether or not to block remote queries of this computer’s index.|
|searchDisableUseLocation|Boolean|Specifies if search can use location information.|
|searchDisableIndexerBackoff|Boolean|Indicates whether or not to disable the search indexer backoff feature.|
|searchDisableIndexingRemovableDrive|Boolean|Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.|
|searchEnableAutomaticIndexSizeManangement|Boolean|Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.|
|searchBlockWebResults|Boolean|Indicates whether or not to block the web search.|
|securityBlockAzureADJoinedDevicesAutoEncryption|Boolean|Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune_deviceconfig_diagnosticdatasubmissionmode.md)|Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson. Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Boolean|Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.|
|systemTelemetryProxyServer|String|Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.|
|inkWorkspaceAccess|[inkAccessSetting](../resources/intune_deviceconfig_inkaccesssetting.md)|Controls the user access to the ink workspace, from the desktop and from above the lock screen. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|inkWorkspaceBlockSuggestedApps|Boolean|Specify whether to show recommended app suggestions in the ink workspace.|
|smartScreenEnableAppInstallControl|Boolean|Allows IT Admins to control whether users are allowed to install apps from places other than the Store.|
|personalizationDesktopImageUrl|String|A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.|
|personalizationLockScreenImageUrl|String|A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.|
|bluetoothAllowedServices|String collection|Specify a list of allowed Bluetooth services and profiles in hex formatted strings.|
|bluetoothBlockAdvertising|Boolean|Whether or not to Block the user from using bluetooth advertising.|
|bluetoothBlockDiscoverableMode|Boolean|Whether or not to Block the user from using bluetooth discoverable mode.|
|bluetoothBlockPrePairing|Boolean|Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.|
|edgeBlockAutofill|Boolean|Indicates whether or not to block auto fill.|
|edgeBlocked|Boolean|Indicates whether or not to Block the user from using the Edge browser.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune_deviceconfig_edgecookiepolicy.md)|Indicates which cookies to block in the Edge browser. Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Boolean|Indicates whether or not to block developer tools in the Edge browser.|
|edgeBlockSendingDoNotTrackHeader|Boolean|Indicates whether or not to Block the user from sending the do not track header.|
|edgeBlockExtensions|Boolean|Indicates whether or not to block extensions in the Edge browser.|
|edgeBlockInPrivateBrowsing|Boolean|Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.|
|edgeBlockJavaScript|Boolean|Indicates whether or not to Block the user from using JavaScript.|
|edgeBlockPasswordManager|Boolean|Indicates whether or not to Block password manager.|
|edgeBlockAddressBarDropdown|Boolean|Block the address bar dropdown functionality in Microsoft Edge. Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.|
|edgeBlockCompatibilityList|Boolean|Block Microsoft compatibility list in Microsoft Edge. This list from Microsoft helps Edge properly display sites with known compatibility issues.|
|edgeClearBrowsingDataOnExit|Boolean|Clear browsing data on exiting Microsoft Edge.|
|edgeAllowStartPagesModification|Boolean|Allow users to change Start pages on Edge. Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.|
|edgeDisableFirstRunPage|Boolean|Block the Microsoft web page that opens on the first use of Microsoft Edge. This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.|
|edgeBlockLiveTileDataCollection|Boolean|Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.|
|edgeSyncFavoritesWithInternetExplorer|Boolean|Enable favorites sync between Internet Explorer and Microsoft Edge. Additions, deletions, modifications and order changes to favorites are shared between browsers.|
|edgeFavoritesListLocation|String|The location of the favorites list to provision. Could be a local file, local network or http location.|
|edgeBlockEditFavorites|Boolean|Indicates whether or not to Block the user from making changes to Favorites.|
|cellularBlockDataWhenRoaming|Boolean|Whether or not to Block the user from using data over cellular while roaming.|
|cellularBlockVpn|Boolean|Whether or not to Block the user from using VPN over cellular.|
|cellularBlockVpnWhenRoaming|Boolean|Whether or not to Block the user from using VPN when roaming over cellular.|
|cellularData|[configurationUsage](../resources/intune_deviceconfig_configurationusage.md)|Whether or not to allow the cellular data channel on the device. If not configured, the cellular data channel is allowed and the user can turn it off. Possible values are: `blocked`, `required`, `allowed`.|
|defenderBlockEndUserAccess|Boolean|Whether or not to block end user access to Defender.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Number of days before deleting quarantined malware. Valid values 0 to 90|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|Gets or sets Defender’s actions to take on detected Malware per threat level.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune_deviceconfig_weeklyschedule.md)|Defender day of the week for the system scan. Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|defenderFilesAndFoldersToExclude|String collection|Files and folder to exclude from scans and real time protection.|
|defenderFileExtensionsToExclude|String collection|File extensions to exclude from scans and real time protection.|
|defenderScanMaxCpu|Int32|Max CPU usage percentage during scan. Valid values 0 to 100|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune_deviceconfig_defendermonitorfileactivity.md)|Value for monitoring file activity. Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderPotentiallyUnwantedAppAction|[defenderPotentiallyUnwantedAppAction](../resources/intune_deviceconfig_defenderpotentiallyunwantedappaction.md)|Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself. Added in Windows 10 for desktop. Possible values are: `deviceDefault`, `block`, `audit`.|
|defenderProcessesToExclude|String collection|Processes to exclude from scans and real time protection.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune_deviceconfig_defenderpromptforsamplesubmission.md)|The configuration for how to prompt user for sample submission. Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Boolean|Indicates whether or not to require behavior monitoring.|
|defenderRequireCloudProtection|Boolean|Indicates whether or not to require cloud protection.|
|defenderRequireNetworkInspectionSystem|Boolean|Indicates whether or not to require network inspection system.|
|defenderRequireRealTimeMonitoring|Boolean|Indicates whether or not to require real time monitoring.|
|defenderScanArchiveFiles|Boolean|Indicates whether or not to scan archive files.|
|defenderScanDownloads|Boolean|Indicates whether or not to scan downloads.|
|defenderScanNetworkFiles|Boolean|Indicates whether or not to scan files opened from a network folder.|
|defenderScanIncomingMail|Boolean|Indicates whether or not to scan incoming mail messages.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean|Indicates whether or not to scan mapped network drives during full scan.|
|defenderScanRemovableDrivesDuringFullScan|Boolean|Indicates whether or not to scan removable drives during full scan.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Indicates whether or not to scan scripts loaded in Internet Explorer browser.|
|defenderSignatureUpdateIntervalInHours|Int32|The signature update interval in hours. Specify 0 not to check. Valid values 0 to 24|
|defenderScanType|[defenderScanType](../resources/intune_deviceconfig_defenderscantype.md)|The defender system scan type. Possible values are: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|The defender time for the system scan.|
|defenderScheduledQuickScanTime|TimeOfDay|The time to perform a daily quick scan.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune_deviceconfig_defendercloudblockleveltype.md)|Specifies the level of cloud-delivered protection. Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeout|Int32|Timeout extension for file scanning by the cloud. Valid values 0 to 50|
|defenderBlockOnAccessProtection|Boolean|Allows or disallows Windows Defender On Access Protection functionality.|
|defenderScheduleScanDay|[defenderScheduleScanDay](../resources/intune_deviceconfig_defenderschedulescanday.md)|Selects the day that the Windows Defender scan should run. Possible values are: `everyday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`, `noScheduledScan`.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune_deviceconfig_defendersubmitsamplesconsenttype.md)|Checks for the user consent level in Windows Defender to send data. Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|lockScreenAllowTimeoutConfiguration|Boolean|Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices. If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.|
|lockScreenBlockActionCenterNotifications|Boolean|Indicates whether or not to block action center notifications over lock screen.|
|lockScreenBlockCortana|Boolean|Indicates whether or not the user can interact with Cortana using speech while the system is locked.|
|lockScreenBlockToastNotifications|Boolean|Indicates whether to allow toast notifications above the device lock screen.|
|lockScreenTimeoutInSeconds|Int32|Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices. Supported values are 11-1800. Valid values 11 to 1800|
|passwordBlockSimple|Boolean|Specify whether PINs or passwords such as "1111" or "1234" are allowed. For Windows 10 desktops, it also controls the use of picture passwords.|
|passwordExpirationDays|Int32|The password expiration in days. Valid values 0 to 730|
|passwordMinimumLength|Int32|The minimum password length. Valid values 4 to 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|The minutes of inactivity before the screen times out.|
|passwordMinimumCharacterSetCount|Int32|The number of character sets required in the password.|
|passwordPreviousPasswordBlockCount|Int32|The number of previous passwords to prevent reuse of. Valid values 0 to 50|
|passwordRequired|Boolean|Indicates whether or not to require the user to have a password.|
|passwordRequireWhenResumeFromIdleState|Boolean|Indicates whether or not to require a password upon resuming from an idle state.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|The required password type. Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|The number of sign in failures before factory reset. Valid values 0 to 999|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Enables or disables the use of advertising ID. Added in Windows 10, version 1607. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.|
|privacyBlockInputPersonalization|Boolean|Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.|
|privacyBlockPublishUserActivities|Boolean|Blocks the shared experiences/discovery of recently used resources in task switcher etc.|
|privacyBlockActivityFeed|Boolean|Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications|
|startBlockUnpinningAppsFromTaskbar|Boolean|Indicates whether or not to block the user from unpinning apps from taskbar.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune_deviceconfig_windowsstartmenuapplistvisibilitytype.md)|Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app. Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Boolean|Enabling this policy hides the change account setting from appearing in the user tile in the start menu.|
|startMenuHideFrequentlyUsedApps|Boolean|Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.|
|startMenuHideHibernate|Boolean|Enabling this policy hides hibernate from appearing in the power button in the start menu.|
|startMenuHideLock|Boolean|Enabling this policy hides lock from appearing in the user tile in the start menu.|
|startMenuHidePowerButton|Boolean|Enabling this policy hides the power button from appearing in the start menu.|
|startMenuHideRecentJumpLists|Boolean|Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.|
|startMenuHideRecentlyAddedApps|Boolean|Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.|
|startMenuHideRestartOptions|Boolean|Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.|
|startMenuHideShutDown|Boolean|Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.|
|startMenuHideSignOut|Boolean|Enabling this policy hides sign out from appearing in the user tile in the start menu.|
|startMenuHideSleep|Boolean|Enabling this policy hides sleep from appearing in the power button in the start menu.|
|startMenuHideSwitchAccount|Boolean|Enabling this policy hides switch account from appearing in the user tile in the start menu.|
|startMenuHideUserTile|Boolean|Enabling this policy hides the user tile from appearing in the start menu.|
|startMenuLayoutEdgeAssetsXml|Binary|This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy. Start layout can contain secondary tile from Edge app which looks for Edge local asset file. Edge local asset would not exist and cause Edge secondary tile to appear empty in this case. This policy only gets applied when startMenuLayoutXml policy is modified. The value should be a UTF-8 Base64 encoded byte array.|
|startMenuLayoutXml|Binary|Allows admins to override the default Start menu layout and prevents the user from changing it. The layout is modified by specifying an XML file based on a layout modification schema. XML needs to be in a UTF8 encoded byte array format.|
|startMenuMode|[windowsStartMenuModeType](../resources/intune_deviceconfig_windowsstartmenumodetype.md)|Allows admins to decide how the Start menu is displayed. Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Boolean|Indicates whether or not to block access to Settings app.|
|settingsBlockSystemPage|Boolean|Indicates whether or not to block access to System in Settings app.|
|settingsBlockDevicesPage|Boolean|Indicates whether or not to block access to Devices in Settings app.|
|settingsBlockNetworkInternetPage|Boolean|Indicates whether or not to block access to Network & Internet in Settings app.|
|settingsBlockPersonalizationPage|Boolean|Indicates whether or not to block access to Personalization in Settings app.|
|settingsBlockAccountsPage|Boolean|Indicates whether or not to block access to Accounts in Settings app.|
|settingsBlockTimeLanguagePage|Boolean|Indicates whether or not to block access to Time & Language in Settings app.|
|settingsBlockEaseOfAccessPage|Boolean|Indicates whether or not to block access to Ease of Access in Settings app.|
|settingsBlockPrivacyPage|Boolean|Indicates whether or not to block access to Privacy in Settings app.|
|settingsBlockUpdateSecurityPage|Boolean|Indicates whether or not to block access to Update & Security in Settings app.|
|settingsBlockAppsPage|Boolean|Indicates whether or not to block access to Apps in Settings app.|
|settingsBlockGamingPage|Boolean|Indicates whether or not to block access to Gaming in Settings app.|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolean|Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.|
|windowsSpotlightBlocked|Boolean|Allows IT admins to turn off all Windows Spotlight features|
|windowsSpotlightBlockOnActionCenter|Boolean|Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed|
|windowsSpotlightBlockTailoredExperiences|Boolean|Block personalized content in Windows spotlight based on user’s device usage.|
|windowsSpotlightBlockThirdPartyNotifications|Boolean|Block third party content delivered via Windows Spotlight|
|windowsSpotlightBlockWelcomeExperience|Boolean|Block Windows Spotlight Windows welcome experience|
|windowsSpotlightBlockWindowsTips|Boolean|Allows IT admins to turn off the popup of Windows Tips.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune_deviceconfig_windowsspotlightenablementsettings.md)|Specifies the type of Spotlight. Possible values are: `notConfigured`, `disabled`, `enabled`.|
|networkProxyApplySettingsDeviceWide|Boolean|If set, proxy settings will be applied to all processes and accounts in the device. Otherwise, it will be applied to the user account that’s enrolled into MDM.|
|networkProxyDisableAutoDetect|Boolean|Disable automatic detection of settings. If enabled, the system will try to find the path to a proxy auto-config (PAC) script.|
|networkProxyAutomaticConfigurationUrl|String|Address to the proxy auto-config (PAC) script you want to use.|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune_deviceconfig_windows10networkproxyserver.md)|Specifies manual proxy server settings.|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.|
|antiTheftModeBlocked|Boolean|Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).|
|bluetoothBlocked|Boolean|Whether or not to Block the user from using bluetooth.|
|cameraBlocked|Boolean|Whether or not to Block the user from accessing the camera of the device.|
|connectedDevicesServiceBlocked|Boolean|Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.|
|certificatesBlockManualRootCertificateInstallation|Boolean|Whether or not to Block the user from doing manual root certificate installation.|
|copyPasteBlocked|Boolean|Whether or not to Block the user from using copy paste.|
|cortanaBlocked|Boolean|Whether or not to Block the user from using Cortana.|
|deviceManagementBlockFactoryResetOnMobile|Boolean|Indicates whether or not to Block the user from resetting their phone.|
|deviceManagementBlockManualUnenroll|Boolean|Indicates whether or not to Block the user from doing manual un-enrollment from device management.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune_deviceconfig_safesearchfiltertype.md)|Specifies what filter level of safe search is required. Possible values are: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Boolean|Indicates whether or not to block popups.|
|edgeBlockSearchSuggestions|Boolean|Indicates whether or not to Block the user from using the search suggestions in the address bar.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolean|Indicates whether or not to Block the user from sending Intranet traffic to Internet Explorer from Edge.|
|edgeRequireSmartScreen|Boolean|Indicates whether or not to Require the user to use the smart screen filter.|
|edgeEnterpriseModeSiteListLocation|String|Indicates the enterprise mode site list location. Could be a local file, local network or http location.|
|edgeFirstRunUrl|String|The first run URL for when Edge browser is opened for the first time.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)|Allows IT admins to set a default search engine for MDM-Controlled devices. Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.|
|edgeHomepageUrls|String collection|The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.|
|edgeBlockAccessToAboutFlags|Boolean|Indicates whether or not to prevent access to about flags on Edge browser.|
|smartScreenBlockPromptOverride|Boolean|Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.|
|smartScreenBlockPromptOverrideForFiles|Boolean|Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files|
|webRtcBlockLocalhostIpAddress|Boolean|Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC|
|internetSharingBlocked|Boolean|Indicates whether or not to Block the user from using internet sharing.|
|settingsBlockAddProvisioningPackage|Boolean|Indicates whether or not to block the user from installing provisioning packages.|
|settingsBlockRemoveProvisioningPackage|Boolean|Indicates whether or not to block the runtime configuration agent from removing provisioning packages.|
|settingsBlockChangeSystemTime|Boolean|Indicates whether or not to block the user from changing date and time settings.|
|settingsBlockEditDeviceName|Boolean|Indicates whether or not to block the user from editing the device name.|
|settingsBlockChangeRegion|Boolean|Indicates whether or not to block the user from changing the region settings.|
|settingsBlockChangeLanguage|Boolean|Indicates whether or not to block the user from changing the language settings.|
|settingsBlockChangePowerSleep|Boolean|Indicates whether or not to block the user from changing power and sleep settings.|
|locationServicesBlocked|Boolean|Indicates whether or not to Block the user from location services.|
|microsoftAccountBlocked|Boolean|Indicates whether or not to Block a Microsoft account.|
|microsoftAccountBlockSettingsSync|Boolean|Indicates whether or not to Block Microsoft account settings sync.|
|nfcBlocked|Boolean|Indicates whether or not to Block the user from using near field communication.|
|resetProtectionModeBlocked|Boolean|Indicates whether or not to Block the user from reset protection mode.|
|screenCaptureBlocked|Boolean|Indicates whether or not to Block the user from taking Screenshots.|
|storageBlockRemovableStorage|Boolean|Indicates whether or not to Block the user from using removable storage.|
|storageRequireMobileDeviceEncryption|Boolean|Indicating whether or not to require encryption on a mobile device.|
|usbBlocked|Boolean|Indicates whether or not to Block the user from USB connection.|
|voiceRecordingBlocked|Boolean|Indicates whether or not to Block the user from voice recording.|
|wiFiBlockAutomaticConnectHotspots|Boolean|Indicating whether or not to block automatically connecting to Wi-Fi hotspots. Has no impact if Wi-Fi is blocked.|
|wiFiBlocked|Boolean|Indicates whether or not to Block the user from using Wi-Fi.|
|wiFiBlockManualConfiguration|Boolean|Indicates whether or not to Block the user from using Wi-Fi manual configuration.|
|wiFiScanInterval|Int32|Specify how often devices scan for Wi-Fi networks. Supported values are 1-500, where 100 = default, and 500 = low frequency. Valid values 1 to 500|
|wirelessDisplayBlockProjectionToThisDevice|Boolean|Indicates whether or not to allow other devices from discovering this PC for projection.|
|wirelessDisplayBlockUserInputFromReceiver|Boolean|Indicates whether or not to allow user input from wireless display receiver.|
|wirelessDisplayRequirePinForPairing|Boolean|Indicates whether or not to require a PIN for new devices to initiate pairing.|
|windowsStoreBlocked|Boolean|Indicates whether or not to Block the user from using the Windows store.|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Boolean|Indicates whether or not to block automatic update of apps from Windows Store.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Indicates whether or not to allow developer unlock. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Boolean|Indicates whether or not to block multiple users of the same app to share data.|
|appsBlockWindowsStoreOriginatedApps|Boolean|Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.|
|windowsStoreEnablePrivateStoreOnly|Boolean|Indicates whether or not to enable Private Store Only.|
|storageRestrictAppDataToSystemVolume|Boolean|Indicates whether application data is restricted to the system drive.|
|storageRestrictAppInstallToSystemVolume|Boolean|Indicates whether the installation of applications is restricted to the system drive.|
|gameDvrBlocked|Boolean|Indicates whether or not to block DVR and broadcasting.|
|experienceBlockDeviceDiscovery|Boolean|Indicates whether or not to enable device discovery UX.|
|experienceBlockErrorDialogWhenNoSIM|Boolean|Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.|
|experienceBlockTaskSwitcher|Boolean|Indicates whether or not to enable task switching on the device.|
|logonBlockFastUserSwitching|Boolean|Disables the ability to quickly switch between users that are logged on simultaneously without logging off.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignedAccessMultiModeProfiles|[windowsAssignedAccessProfile](../resources/intune_deviceconfig_windowsassignedaccessprofile.md) collection|This policy setting allows to define a list of assigned access profiles for multi app mode.|
|privacyAccessControls|[windowsPrivacyDataAccessControlItem](../resources/intune_deviceconfig_windowsprivacydataaccesscontrolitem.md) collection|Indicates a list of applications with their access control levels over privacy data categories, and/or the default access levels per category.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "enableAutomaticRedeployment": true,
  "assignedAccessSingleModeUserName": "String",
  "assignedAccessSingleModeAppUserModelId": "String",
  "microsoftAccountSignInAssistantSettings": "String",
  "authenticationAllowSecondaryDevice": true,
  "authenticationAllowFIDODevice": true,
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "String"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "String"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "String",
  "enterpriseCloudPrintOAuthAuthority": "String",
  "enterpriseCloudPrintOAuthClientIdentifier": "String",
  "enterpriseCloudPrintResourceIdentifier": "String",
  "enterpriseCloudPrintDiscoveryMaxLimit": 1024,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "String",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "String"
  ],
  "printerDefaultName": "String",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "String",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "String",
  "inkWorkspaceAccess": "String",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "String",
  "personalizationLockScreenImageUrl": "String",
  "bluetoothAllowedServices": [
    "String"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "String",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "String",
  "edgeBlockEditFavorites": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "String",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  },
  "defenderSystemScanSchedule": "String",
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderScanMaxCpu": 1024,
  "defenderMonitorFileActivity": "String",
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPromptForSampleSubmission": "String",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderScanType": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeout": 1024,
  "defenderBlockOnAccessProtection": true,
  "defenderScheduleScanDay": "String",
  "defenderSubmitSamplesConsentType": "String",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 1024,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "privacyAdvertisingId": "String",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "String",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "binary",
  "startMenuLayoutXml": "binary",
  "startMenuMode": "String",
  "startMenuPinnedFolderDocuments": "String",
  "startMenuPinnedFolderDownloads": "String",
  "startMenuPinnedFolderFileExplorer": "String",
  "startMenuPinnedFolderHomeGroup": "String",
  "startMenuPinnedFolderMusic": "String",
  "startMenuPinnedFolderNetwork": "String",
  "startMenuPinnedFolderPersonalFolder": "String",
  "startMenuPinnedFolderPictures": "String",
  "startMenuPinnedFolderSettings": "String",
  "startMenuPinnedFolderVideos": "String",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "String",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "String",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "String",
    "exceptions": [
      "String"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "String",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "String",
  "edgeFirstRunUrl": "String",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "String"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 1024,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "String",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "String",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```



