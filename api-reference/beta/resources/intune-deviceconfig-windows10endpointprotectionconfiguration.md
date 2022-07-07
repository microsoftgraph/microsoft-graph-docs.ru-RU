---
title: Тип ресурса windows10EndpointProtectionConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом Windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51d7efa1cd041c3aa4aa995da2ecfec045d8995a
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670409"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>Тип ресурса windows10EndpointProtectionConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом Windows10EndpointProtectionConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|Коллекция [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Перечисление свойств и связей объектов [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Получение объекта windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Чтение свойств и связей объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Создание объекта windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Удаление объекта windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|Нет|Удаление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Обновление объекта windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Обновление свойств объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|Эта политика предназначена для обеспечения дополнительной безопасности внешних устройств с поддержкой DMA. Он обеспечивает более полный контроль над перечислением внешних устройств с поддержкой DMA, несовместимых с изоляцией памяти dMA Remapping и изолированием памяти устройства и песочницей. Эта политика вступает в силу только в том случае, если встроенное ПО системы поддерживает защиту DMA ядра. Защита DMA ядра — это функция платформы, которая не может управляться политикой или конечным пользователем. Он должен поддерживаться системой во время производства. Чтобы проверить, поддерживает ли система защиту DMA ядра, проверьте поле "Защита DMA ядра" на странице сводки MSINFO32.exe. Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.|
|firewallRules|[Коллекция windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)|Настраивает параметры правил брандмауэра. Эта коллекция может содержать не более 150 элементов.|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления. Сохраненные учетные данные пользователей могут быть скомпрометированными, если эта привилегия предоставляется другим сущностям. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру по сети. Поддерживается состояние "Разрешено".|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы блокируют подключение к компьютеру по сети. Блок состояния поддерживается.|
|UserRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности. Таким образом, этот процесс может получить доступ к тем же локальным ресурсам, что и этот пользователь. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут войти на компьютер. Поддерживаются состояния NotConfigured, Allowed |
|userRightsDenyLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи не могут войти на компьютер. Поддерживаются состояния NotConfigured, Blocked |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут обходить разрешения файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутренних часах компьютера. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов. Пользователи, которые могут создавать глобальные объекты, могут влиять на процессы, которые выполняются в сеансах других пользователей, что может привести к сбою приложения или повреждению данных. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API для создания и изменения размера файла страницы. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, может ли пользователь создать символьную ссылку с компьютера, на который он вошел. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи или группы могут использоваться процессами для создания маркера, который затем может использоваться для получения доступа к любым локальным ресурсам, когда процесс использует внутренний API для создания маркера доступа. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут присоединить отладчик к любому процессу или ядру. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы запрещены для входа в качестве клиента служб удаленных рабочих столов. Поддерживаются только состояния NotConfigured и Blocked|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут устанавливать параметр "Доверенный для делегирования" для объекта пользователя или компьютера. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности. Журнал безопасности используется для трассировки несанкционированного доступа к системе.  Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Назначение этого права пользователю позволяет программам, запущенным от имени этого пользователя, олицетворять клиент. Требование этого права пользователя для такого олицетворения предотвращает несанкционированный пользователь от несанкционированного подключения клиента к созданной им службе, а затем олицетворения этого клиента, что может повысить разрешения неавторизованного пользователя до административных или системных уровней. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом свойства записи к другому процессу, чтобы увеличить приоритет выполнения, назначенный другому процессу. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что не позволяет системе разбиение данных на виртуальную память на диске. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут указывать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания на томе, например удаленную дефрагментацию. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, кто может изменять значения среды встроенного ПО. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи пользователей могут изменять метку целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для мониторинга производительности системных процессов. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут завершить работу компьютера из удаленного расположения в сети. Неправильное использование этого права пользователя может привести к отказу в обслуживании. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут обходить разрешения файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, а также определяет, какие пользователи могут установить любой допустимый субъект безопасности в качестве владельца объекта. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут быть владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки. Поддерживаются только состояния NotConfigured и Allowed.|
|xboxServicesEnableXboxGameSaveTask|Логическое|Этот параметр определяет, включено ли сохранение игры Xbox (1) или отключено (0).|
|xboxServicesAccessoryManagementServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска службы управления аксессуарами автоматическим (2), вручную (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|XboxServicesLiveAuthManagerServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет тип запуска службы Live Auth Manager — Automatic(2), Manual(3), Disabled(4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|XboxServicesLiveGameSaveServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, имеет ли служба live Game тип запуска Automatic(2), Manual(3), Disabled(4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|XboxServicesLiveNetworkingServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет тип запуска сетевой службы Automatic(2), Manual(3), Disabled(4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|localSecurityOptionsBlockMicrosoftAccounts|Логическое|Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Логическое|Включите локальные учетные записи, которые не защищены паролем, для входа из расположений, отличных от физического устройства. Включено значение по умолчанию|
|localSecurityOptionsDisableAdministratorAccount|Логическое|Определяет, включена или отключена учетная запись локального администратора.|
|localSecurityOptionsAdministratorAccountName|String|Определите другое имя учетной записи, которое будет связано с идентификатором безопасности (SID) для учетной записи "Администратор".|
|localSecurityOptionsDisableGuestAccount|Логическое|Определяет, включена или отключена гостевая учетная запись.|
|localSecurityOptionsGuestAccountName|String|Определите другое имя учетной записи, которое будет связано с идентификатором безопасности (SID) для учетной записи Guest.|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Логическое|Запретить открепление переносимого компьютера без необходимости входа в систему.|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Логическое|Ограничив установку драйверов принтера в рамках подключения к общему принтеру только администраторам.|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Логическое|Включение этого параметра позволяет только пользователю, вошедаму в систему в интерактивном режиме, получать доступ к компакт-диску.|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|Определите, кому разрешено форматировать и удалять съемные носители NTFS. Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsMachineInactivityLimit|Int32|Определите максимальное время бездействия в минутах на экране входа интерактивного рабочего стола до запуска средства сохранения экрана. Допустимые значения от 0 до 9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|Определите максимальное время бездействия в минутах на экране входа интерактивного рабочего стола до запуска средства сохранения экрана. Допустимые значения от 0 до 9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|Логическое|Прежде чем пользователь сможет войти в систему, необходимо нажать клавиши CTRL+ALT+DEL.|
|localSecurityOptionsHideLastSignedInUser|Логическое|Не отображайте имя пользователя последнего пользователя, выполнившего вход на этом устройстве.|
|localSecurityOptionsHideUsernameAtSignIn|Логическое|Не отображайте имя пользователя, войдите на это устройство после ввода учетных данных и перед отображением рабочего стола устройства.|
|localSecurityOptionsLogOnMessageTitle|String|Задайте заголовок сообщения для пользователей, которые пытаются войти в систему.|
|localSecurityOptionsLogOnMessageText|String|Задайте текст сообщения для пользователей, пытающийся войти в систему.|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Логическое|Блокировать запросы проверки подлинности PKU2U к этому устройству для использования сетевых удостоверений.|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Логическое|Логическое значение вспомогательного интерфейса для сущности LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|Измените строку языка определения дескриптора безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам выполнять удаленные вызовы SAM.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Этот параметр безопасности позволяет клиенту требовать согласования 128-разрядного шифрования и (или) безопасности сеанса NTLMv2. Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Этот параметр безопасности позволяет серверу требовать согласования 128-разрядного шифрования и (или) безопасности сеанса NTLMv2. Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|Этот параметр безопасности определяет, какой протокол проверки подлинности запроса/ответа используется для сетевых входов. Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.|
|lanManagerWorkstationDisableInsecureGuestLogons|Логическое|Если этот параметр включен, клиент SMB разрешит небезопасные гостевые входы. Если этот параметр не настроен, клиент SMB отклонит небезопасные гостевые входы.|
|localSecurityOptionsClearVirtualMemoryPageFile|Логическое|Этот параметр безопасности определяет, очищается ли файл pagefile виртуальной памяти при завершении работы системы.|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Логическое|Этот параметр безопасности определяет, можно ли завершить работу компьютера без необходимости входа в Windows.|
|localSecurityOptionsAllowUIAccessApplicationElevation|Логическое|Разрешите приложениям UIAccess запрашивать повышение прав без использования безопасного рабочего стола.|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Логическое|Сбои записи файлов и реестра в виртуализацию для каждого пользователя|
|localSecurityOptionsOnlyElevateSignedExecutables|Логический|Принудительно выполните проверку пути сертификации PKI для заданного исполняемого файла, прежде чем он будет разрешен для запуска.|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|Определите поведение запроса на повышение прав для администраторов в Администратор утверждения. Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|Определите поведение запроса на повышение прав для обычных пользователей. Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Логический|Включите все запросы на повышение прав для перехода на рабочий стол интерактивного пользователя, а не на безопасный рабочий стол. Используются параметры политики поведения запросов для администраторов и обычных пользователей.|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Логическое|При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено значение по умолчанию|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Логическое|Разрешите приложениям UIAccess запрашивать повышение прав без использования безопасного рабочего стола. Включено значение по умолчанию|
|localSecurityOptionsUseAdminApprovalMode|Логическое|Определяет, использует ли встроенная учетная запись администратора Администратор режим утверждения или все приложения с полными правами администратора. Включено значение по умолчанию|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Логическое|Определите, Администратор режим утверждения и все параметры политики UAC включены, включено ли значение по умолчанию|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|Настройте сведения о пользователе, отображаемые при блокировке сеанса. Если этот параметр не настроен, отображаются отображаемое имя пользователя, домен и имя пользователя. Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|Настройте сведения о пользователе, отображаемые при блокировке сеанса. Если этот параметр не настроен, отображаются отображаемое имя пользователя, домен и имя пользователя. Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Логическое|Этот параметр безопасности определяет, пытается ли клиент SMB согласовать подписывание пакетов SMB.|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Логическое|Этот параметр безопасности определяет, требуется ли подписывание пакетов клиентским компонентом SMB.|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Логическое|Если этот параметр безопасности включен, перенаправлению SMB разрешается отправлять пароли в виде открытого текста на серверы SMB сторонних поставщиков, которые не поддерживают шифрование паролей во время проверки подлинности.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Логическое|Этот параметр безопасности определяет, требуется ли подписывание пакетов компонентом сервера SMB.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Логическое|Этот параметр безопасности определяет, будет ли сервер SMB согласовывать подписывание пакетов SMB с клиентами, которые запрашивают его.|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Логическое|По умолчанию этот параметр безопасности ограничивает анонимный доступ к общим папкам и каналам для параметров именованных каналов, к которые можно получить анонимный доступ, и к общим папкам, к которые можно получить анонимный доступ.|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Логическое|Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены для анонимных подключений к компьютеру.|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Логическое|Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, такие как перечисление имен учетных записей домена и сетевых ресурсов.|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Логическое|Этот параметр безопасности определяет, сохраняется ли при следующем изменении пароля хэш-значение lan Manager (LM) для нового пароля. Он не хранится по умолчанию.|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);|Этот параметр безопасности определяет, что происходит при удалении смарт-карты для пользователя, выполнив вход в систему, из средства чтения смарт-карт. Возможные значения: `noAction`, `lockWorkstation`, `forceLogoff`, `disconnectRemoteDesktopSession`.|
|defenderSecurityCenterDisableAppBrowserUI|Логический|Используется для отключения отображения области защиты приложения и браузера.|
|defenderSecurityCenterDisableFamilyUI|Логическое|Используется для отключения отображения области параметров семейства.|
|defenderSecurityCenterDisableHealthUI|Логическое|Используется для отключения отображения области производительности и работоспособности устройства.|
|defenderSecurityCenterDisableNetworkUI|Логическое|Используется для отключения отображения брандмауэра и области защиты сети.|
|defenderSecurityCenterDisableVirusUI|Логическое|Используется для отключения отображения области защиты от вирусов и угроз.|
|defenderSecurityCenterDisableAccountUI|Логическое|Используется для отключения отображения области защиты учетной записи.|
|defenderSecurityCenterDisableClearTpmUI|Логическое|Используется для отключения отображения кнопки очистки доверенного платформенного модуля.|
|defenderSecurityCenterDisableHardwareUI|Логическое|Используется для отключения отображения области защиты оборудования.|
|defenderSecurityCenterDisableNotificationAreaUI|Логическое|Используется для отключения отображения элемента управления области уведомлений. Чтобы этот параметр вступает в силу, пользователю необходимо выйти и войти в систему или перезагрузить компьютер.|
|defenderSecurityCenterDisableRansomwareUI|Логическое|Используется для отключения отображения области защиты программ-шантажистов. |
|defenderSecurityCenterDisableSecureBootUI|Логическое|Используется для отключения отображения безопасной области загрузки в разделе "Безопасность устройства".|
|DefenderSecurityCenterDisableTroubleshootingUI|Логическое|Используется для отключения отображения устранения неполадок процесса безопасности в разделе "Безопасность устройства".|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|Логическое|Используется для отключения отображения обновления встроенного ПО доверенного платформенного модуля при обнаружении уязвимого встроенного ПО.|
|defenderSecurityCenterOrganizationDisplayName|String|Название компании, отображаемое пользователям.|
|defenderSecurityCenterHelpEmail|String|Адрес электронной почты, отображаемый пользователям.|
|defenderSecurityCenterHelpPhone|String|Номер телефона или идентификатор Skype, отображаемый пользователям.|
|defenderSecurityCenterHelpURL|String|URL-адрес портала справки, который отображается для пользователей.|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|Уведомления, отображаемые из отображаемых областей приложения. Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|Настройка расположения для отображения контактных данных ИТ-служб для конечных пользователей. Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.|
|windowsDefenderTamperProtection|[windowsDefenderTamperProtectionOptions](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|Настройка параметров TamperProtection в Защитнике Windows. Возможные значения: `notConfigured`, `enable`, `disable`.|
|firewallBlockStatefulFTP|Boolean|Блокирует FTP-подключения к устройству с отслеживанием состояния.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно. По истечении этого срока сопоставления безопасности перестают действовать и удаляются. Допустимые значения: от 300 до 3600|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|Выберите кодировку предварительно используемого ключа. Возможные значения: `deviceDefault`, `none`, `utF8`.|
|firewallIPSecExemptionsNone|Логический|Настраивает исключения IPSec без исключений|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.|
|firewallIPSecExemptionsAllowICMP|Boolean|Настраивает исключения IPSec для разрешения ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.|
|firewallIPSecExemptionsAllowDHCP|Boolean|Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|Укажите способ применения списка отзыва сертификатов. Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Boolean|Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|Настраивает способ применения очередей пакетов в сценарии шлюза туннеля. Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для доменных сетей|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для общедоступных сетей|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для частных сетей|
|defenderAdobeReaderLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение Adobe Reader при создании дочерних процессов. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderAttackSurfaceReductionExcludedPaths|Коллекция String|Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение приложений Office, внедряющихся в другие процессы. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение приложений Office, внедряющихся в другие процессы. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeCommunicationAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение информационных приложений Office, включая Microsoft Outlook, от создания дочерних процессов. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого содержимого. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого содержимого. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение приложения Office, запускающего дочерние процессы. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение приложения Office, запускающего дочерние процессы. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение импорта Win32 из кода макроса в Office. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение импорта Win32 из кода макроса в Office. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение замаскированных кодов js/vbs/ps/macro. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение замаскированных кодов js/vbs/ps/macro. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение js/vbs, выполняющее полезные данные, скачанных из Интернета. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение js/vbs, выполняющее полезные данные, скачанных из Интернета. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее, разрешен ли кража учетных данных из подсистемы локального центра безопасности Windows. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее ответ на создание процессов из команд PSExec и WMI. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее ответ на создание процессов из команд PSExec и WMI. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее ответ на ненадежные и неподписаные процессы, которые выполняются из USB. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее ответ на ненадежные и неподписаные процессы, которые выполняются из USB. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее ответ на исполняемые файлы, которые не соответствуют критериям распространенности, возраста или доверенного списка. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее ответ на исполняемые файлы, которые не соответствуют критериям распространенности, возраста или доверенного списка. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее, следует ли удалять исполняемое содержимое (exe, dll, ps, js, vbs и т. д.) из электронной почты (webmail/mail-client). Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее, следует ли удалять исполняемое содержимое (exe, dll, ps, js, vbs и т. д.) из электронной почты (webmail/mail-client). Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее на использование расширенной защиты от программ-шантажистов. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|Значение, указывающее поведение защищенных папок. Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.|
|defenderGuardedFoldersAllowedAppPaths|Коллекция String|Список путей к файлам EXE, которым разрешен доступ к защищенным папкам|
|defenderAdditionalGuardedFolders|Коллекция String|Список путей к папкам, которые следует добавить в список защищенных папок|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение NetworkProtection. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderExploitProtectionXml|Binary|XML-файл с информацией о защите от эксплойтов.|
|defenderExploitProtectionXmlFileName|String|Имя файла, из которого получено свойство DefenderExploitProtectionXml.|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.|
|defenderBlockPersistenceThroughWmiType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение блокировки сохраняемости через подписку на события WMI. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|Позволяет администратору выбирать разрешенные типы приложений для устройств. Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[DeviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|Включите Credential Guard, если включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации. Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.|
|DeviceGuardEnableVirtualizationBasedSecurity|Логическое|Включает безопасность на основе виртуализации (VBS).|
|deviceGuardEnableSecureBootWithDMA|Логическое|Это свойство будет нерекомендуемым в мае 2019 г. и будет заменено свойством DeviceGuardSecureBootWithDMA. Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.|
|deviceGuardSecureBootWithDMA|[secureBootWithDMAType](../resources/intune-deviceconfig-securebootwithdmatype.md)|Указывает, включен ли уровень безопасности платформы при следующей перезагрузке. Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.|
|deviceGuardLaunchSystemGuard|[Включения](../resources/intune-deviceconfig-enablement.md)|Позволяет ИТ-администратору настроить запуск System Guard. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|smartScreenEnableInShell|Boolean|Позволяет ИТ-администраторам настраивать SmartScreen для Windows.|
|smartScreenBlockOverrideForFiles|Boolean|Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.|
|applicationGuardEnabled|Boolean|Включение Application Guard в Защитнике Windows|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|Включите Application Guard в Защитнике Windows для более новых сборок Windows. Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|Блокирование буфера обмена для передачи файла изображения, текстового файла или ни одного из них. Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolean|Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.|
|applicationGuardAllowPersistence|Boolean|Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).|
|applicationGuardForceAuditing|Boolean|Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена. Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolean|Позволяет разрешить печать в PDF из контейнера.|
|applicationGuardAllowPrintToXPS|Boolean|Позволяет разрешить печать в XPS из контейнера.|
|applicationGuardAllowPrintToLocalPrinters|Boolean|Позволяет разрешить печать на локальных принтерах из контейнера.|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|Позволяет разрешить печать на сетевых принтерах из контейнера.|
|applicationGuardAllowVirtualGPU|Логический|Разрешить Application Guard использовать виртуальный GPU|
|applicationGuardAllowFileSaveOnHost|Логическое|Разрешить пользователям скачивать файлы из Edge в контейнер Application Guard и сохранять их в файловой системе узла.|
|applicationGuardAllowCameraMicrophoneRedirection|Логическое|Возвращает или задает, могут ли приложения внутри Application Guard в Microsoft Defender получать доступ к камере и микрофону устройства.|
|applicationGuardCertificateThumbprints|Коллекция String|Позволяет совместно использовать некоторые корневые сертификаты уровня устройства с Application Guard в Microsoft Defender контейнера.|
|bitLockerAllowStandardUserEncryption|Логическое|Позволяет администратору разрешить стандартным пользователям включить encrpytion во время Azure AD join.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|Позволяет администратору требовать включения шифрования с помощью BitLocker. Эта политика действительна только для мобильных устройств.|
|bitLockerEncryptDevice|Boolean|Позволяет администратору требовать включения шифрования с помощью BitLocker.|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|Политика системного диска BitLocker.|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);|Политика фиксированного диска BitLocker.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|Политика BitLocker в отношении съемных дисков.|
|BitLockerRecoveryPasswordRotation|[bitLockerRecoveryPasswordRotationType](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|Этот параметр инициирует смену пароля восстановления на основе клиента после восстановления диска ОС (с помощью bootmgr или WinRE). Возможные значения: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.|
|defenderDisableScanArchiveFiles|Логическое|Разрешает или запрещает сканирование архивов.|
|defenderAllowScanArchiveFiles|Логическое|Разрешает или запрещает сканирование архивов.|
|defenderDisableBehaviorMonitoring|Логическое|Разрешает или запрещает Защитник Windows функции мониторинга поведения.|
|defenderAllowBehaviorMonitoring|Логическое|Разрешает или запрещает Защитник Windows функции мониторинга поведения.|
|defenderDisableCloudProtection|Логическое|Чтобы обеспечить оптимальную защиту компьютера, Защитник Windows отправляет в корпорацию Майкрософт сведения о любых обнаруженных проблемах. Корпорация Майкрософт проанализирует эту информацию, узнает больше о проблемах, влияющих на вас и других клиентов, и предложит улучшенные решения.|
|defenderAllowCloudProtection|Логическое|Чтобы обеспечить оптимальную защиту компьютера, Защитник Windows отправляет в корпорацию Майкрософт сведения о любых обнаруженных проблемах. Корпорация Майкрософт проанализирует эту информацию, узнает больше о проблемах, влияющих на вас и других клиентов, и предложит улучшенные решения.|
|defenderEnableScanIncomingMail|Логическое|Разрешает или запрещает сканирование электронной почты.|
|defenderEnableScanMappedNetworkDrivesDuringFullScan|Логическое|Разрешает или запрещает полную проверку сопоставленных сетевых дисков.|
|defenderDisableScanRemovableDrivesDuringFullScan|Логическое|Разрешает или запрещает полную проверку съемных дисков. Во время быстрой проверки съемные диски могут по-прежнему проверяться.|
|defenderAllowScanRemovableDrivesDuringFullScan|Логическое|Разрешает или запрещает полную проверку съемных дисков. Во время быстрой проверки съемные диски могут по-прежнему проверяться.|
|DefenderDisableScanDownloads|Логическое|Разрешает или запрещает использование Защитник Windows защиты IOAVP.|
|DefenderAllowScanDownloads|Логическое|Разрешает или запрещает использование Защитник Windows защиты IOAVP.|
|defenderDisableIntrusionPreventionSystem|Логическое|Разрешает или запрещает Защитник Windows функции предотвращения вторжений.|
|defenderAllowIntrusionPreventionSystem|Логическое|Разрешает или запрещает Защитник Windows функции предотвращения вторжений.|
|defenderDisableOnAccessProtection|Логическое|Разрешает или запрещает использование Защитник Windows on Access Protection.|
|defenderAllowOnAccessProtection|Логическое|Разрешает или запрещает использование Защитник Windows on Access Protection.|
|defenderDisableRealTimeMonitoring|Логическое|Разрешает или запрещает Защитник Windows мониторинга в режиме реального времени.|
|defenderAllowRealTimeMonitoring|Логическое|Разрешает или запрещает Защитник Windows мониторинга в режиме реального времени.|
|defenderDisableScanNetworkFiles|Логическое|Разрешает или запрещает сканирование сетевых файлов.|
|defenderAllowScanNetworkFiles|Логическое|Разрешает или запрещает сканирование сетевых файлов.|
|defenderDisableScanScriptsLoadedInInternetExplorer|Логическое|Разрешает или запрещает использование Защитник Windows проверки скриптов.|
|defenderAllowScanScriptsLoadedInInternetExplorer|Логическое|Разрешает или запрещает использование Защитник Windows проверки скриптов.|
|defenderBlockEndUserAccess|Boolean|Разрешает или запрещает пользователю доступ к Защитник Windows пользовательского интерфейса. Если запрет запрещен, все Защитник Windows уведомления также будут подавляться.|
|defenderAllowEndUserAccess|Логическое|Разрешает или запрещает пользователю доступ к Защитник Windows пользовательского интерфейса. Если запрет запрещен, все Защитник Windows уведомления также будут подавляться.|
|defenderScanMaxCpuPercentage|Int32|Представляет средний коэффициент загрузки ЦП для Защитник Windows проверки (в процентах). Значение по умолчанию равно 50. Допустимые значения: от 0 до 100|
|defenderCheckForSignaturesBeforeRunningScan|Логический|Этот параметр политики позволяет управлять тем, будет ли выполняться проверка новых определений вирусов и шпионского ПО перед запуском проверки.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Добавлено в Windows 10 версии 1709. Этот параметр политики определяет, насколько антивирусная программа  при блокировке и сканировании подозрительных файлов. Тип значения — целое число. Для работы этой функции необходимо включить параметр "Присоединиться к Microsoft MAPS". Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeoutInSeconds|Int32|Добавлено в Windows 10 версии 1709. Эта функция позволяет антивирусная программа  подозрительный файл на 60 секунд и проверять его в облаке, чтобы убедиться, что он является безопасным. Тип значения — целое число, диапазон — от 0 до 50. Эта функция зависит от трех других параметров MAPS, которые должны быть включены: "Настройка функции "Блокировать при первом появлении"; " Присоединение к Microsoft MAPS"; "Отправка примеров файлов при необходимости дальнейшего анализа". Допустимые значения: от 0 до 50.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Период времени (в днях), в течение которого элементы карантина будут храниться в системе. Допустимые значения: от 0 до 90.|
|defenderDisableCatchupFullScan|Логический|Этот параметр политики позволяет настроить дополнительные проверки для запланированных полных проверок. Перехватывающее сканирование — это проверка, которая инициируется из-за пропущенной регулярной запланированной проверки. Обычно эти запланированные проверки пропускаются, так как компьютер был отключен в запланированное время.|
|defenderDisableCatchupQuickScan|Логическое|Этот параметр политики позволяет настроить дополнительные проверки для запланированных быстрых проверок. Перехватывающее сканирование — это проверка, которая инициируется из-за пропущенной регулярной запланированной проверки. Обычно эти запланированные проверки пропускаются, так как компьютер был отключен в запланированное время.|
|defenderEnableLowCpuPriority|Логическое|Этот параметр политики позволяет включить или отключить низкий приоритет ЦП для запланированных проверок.|
|defenderFileExtensionsToExclude|Коллекция String|Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderFilesAndFoldersToExclude|Коллекция String|Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderProcessesToExclude|Коллекция String|Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderPotentiallyUnwantedAppAction|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Добавлено в Windows 10 версии 1607. Задает уровень обнаружения потенциально нежелательных приложений (PUA). Защитник Windows оповещений о скачиваемом потенциально нежелательном программном обеспечении или попытке установить себя на компьютере. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScanDirection|[defenderRealtimeScanDirection](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|Определяет, какие наборы файлов следует отслеживать. Возможные значения: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Определяет, следует ли выполнять быструю или полную проверку. Возможные значения: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledQuickScanTime|TimeOfDay|Выбирает время суток, в которое должна Защитник Windows быстрая проверка. Например, значение 0=12:00AM, значение 60=1:00AM, значение 120=2:00 и т. д., до значения 1380=11:00PM. Значение по умолчанию — 120|
|defenderScheduledScanDay|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Выбирает день выполнения Защитник Windows проверки. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderScheduledScanTime|TimeOfDay|Выбирает время суток, в течение которого Защитник Windows сканирования.|
|defenderSignatureUpdateIntervalInHours|Int32|Указывает интервал (в часах), который будет использоваться для проверки подписей, поэтому вместо scheduleDay и ScheduleTime проверка новых подписей будет установлена в соответствии с интервалом. Допустимые значения: от 0 до 24.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);|Проверяет уровень согласия пользователя в Защитник Windows для отправки данных. Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Позволяет администратору указать допустимые уровни серьезности угрозы и соответствующий идентификатор действия по умолчанию.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "dmaGuardDeviceEnumerationPolicy": "String",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "String",
      "description": "String",
      "packageFamilyName": "String",
      "filePath": "String",
      "serviceName": "String",
      "protocol": 1024,
      "localPortRanges": [
        "String"
      ],
      "remotePortRanges": [
        "String"
      ],
      "localAddressRanges": [
        "String"
      ],
      "remoteAddressRanges": [
        "String"
      ],
      "profileTypes": "String",
      "action": "String",
      "trafficDirection": "String",
      "interfaceTypes": "String",
      "edgeTraversal": "String",
      "localUserAuthorizations": "String"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "String",
  "xboxServicesLiveAuthManagerServiceStartupMode": "String",
  "xboxServicesLiveGameSaveServiceStartupMode": "String",
  "xboxServicesLiveNetworkingServiceStartupMode": "String",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "String",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
  "localSecurityOptionsMachineInactivityLimit": 1024,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 1024,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "String",
  "localSecurityOptionsLogOnMessageText": "String",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "String",
  "lanManagerAuthenticationLevel": "String",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "String",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "String",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "String",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "String",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "String",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "String",
  "defenderSecurityCenterHelpEmail": "String",
  "defenderSecurityCenterHelpPhone": "String",
  "defenderSecurityCenterHelpURL": "String",
  "defenderSecurityCenterNotificationsFromApp": "String",
  "defenderSecurityCenterITContactDisplay": "String",
  "windowsDefenderTamperProtection": "String",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsNone": true,
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "String",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "String",
  "defenderOfficeAppsLaunchChildProcessType": "String",
  "defenderOfficeAppsLaunchChildProcess": "String",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "String",
  "defenderOfficeMacroCodeAllowWin32Imports": "String",
  "defenderScriptObfuscatedMacroCodeType": "String",
  "defenderScriptObfuscatedMacroCode": "String",
  "defenderScriptDownloadedPayloadExecutionType": "String",
  "defenderScriptDownloadedPayloadExecution": "String",
  "defenderPreventCredentialStealingType": "String",
  "defenderProcessCreationType": "String",
  "defenderProcessCreation": "String",
  "defenderUntrustedUSBProcessType": "String",
  "defenderUntrustedUSBProcess": "String",
  "defenderUntrustedExecutableType": "String",
  "defenderUntrustedExecutable": "String",
  "defenderEmailContentExecutionType": "String",
  "defenderEmailContentExecution": "String",
  "defenderAdvancedRansomewareProtectionType": "String",
  "defenderGuardMyFoldersType": "String",
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderNetworkProtectionType": "String",
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "defenderBlockPersistenceThroughWmiType": "String",
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "String",
  "deviceGuardLaunchSystemGuard": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "String",
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "String"
  ],
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "String",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "String",
    "startupAuthenticationTpmPinUsage": "String",
    "startupAuthenticationTpmKeyUsage": "String",
    "startupAuthenticationTpmPinAndKeyUsage": "String",
    "minimumPinLength": 1024,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "String",
    "prebootRecoveryUrl": "String"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "String",
  "defenderDisableScanArchiveFiles": true,
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 1024,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderScanDirection": "String",
  "defenderScanType": "String",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderScheduledScanDay": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderSubmitSamplesConsentType": "String",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  }
}
```




