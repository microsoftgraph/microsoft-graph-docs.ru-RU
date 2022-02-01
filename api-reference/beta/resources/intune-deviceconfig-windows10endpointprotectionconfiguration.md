---
title: Тип ресурса windows10EndpointProtectionConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом Windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc5d3e4b11abc0838de9debafae2625cc21aad1e
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290891"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>Тип ресурса windows10EndpointProtectionConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом Windows10EndpointProtectionConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

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
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств, способных к DMA. Это позволяет больше контролировать переумывление внешних устройств, способных к DMA, несовместимых с DMA Remapping/device memory isolation and sandboxing. Эта политика вступает в силу только тогда, когда защита DMA ядра поддерживается и включена программным обеспечением системы. Защита DMA ядра — это функция платформы, которая не может управляться с помощью политики или конечным пользователем. Она должна поддерживаться системой во время производства. Чтобы проверить, поддерживает ли система защиту DMA ядра, ознакомьтесь с полем Защиты DMA ядра на странице Сводка MSINFO32.exe. Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.|
|firewallRules|[коллекция windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)|Настраивает параметры правил брандмауэра. Эта коллекция может содержать не более 150 элементов.|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления. Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия будет предоставлена другим сущностям. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру по сети. Разрешено состояние поддерживается.|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы блокируют подключение к компьютеру по сети. Поддерживается государственный блок.|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя позволяет процессу выдать себя любому пользователю без проверки подлинности. Таким образом, этот процесс может получить доступ к тем же локальным ресурсам, что и этот пользователь. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут войти на компьютер. Состояния NotConfigured, Разрешенные поддерживаются |
|userRightsDenyLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи не могут войти на компьютер. Поддерживаются состояния NotConfigured, Blocked |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут обходить разрешения файлов, каталогов, реестров и других постоянных объектов при архивов и каталогах. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутренних часах компьютера. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов. Пользователи, которые могут создавать глобальные объекты, могут влиять на процессы, которые запускаются в сеансах других пользователей, что может привести к сбою приложения или повреждениям данных. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API для создания и изменения размера файла страницы. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи можно использовать в процессах для создания объекта каталога с помощью объекта-диспетчера. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который он вошел. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи/группы могут использоваться процессами для создания маркера, который затем можно использовать для получения доступа к любым локальным ресурсам, когда процесс использует внутренний API для создания маркера доступа. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут прикрепить отладка к любому процессу или к ядру. Поддерживаются только состояния NotConfigured и Allowed|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы не могут войти в систему в качестве клиента служб удаленного рабочего стола. Поддерживаются только состояния NotConfigured и Blocked|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут установить параметр Доверенный для делегирования на объект пользователя или компьютера. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи можно использовать для добавления записей в журнал безопасности. Журнал безопасности используется для отслеживания несанкционированного доступа к системе.  Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Назначение этого права пользователю позволяет программам, работающим от имени этого пользователя, выдать себя за клиента. Требование этого права пользователя для такого обезличения не позволяет неавторизованному пользователю убедить клиента подключиться к созданной им службе, а затем выдать себя за этого клиента, что может привести к повышению разрешений неавторизованного пользователя до административных или системных уровней. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом write Property к другому процессу для увеличения приоритета выполнения, назначенного другому процессу. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут динамически загружать и разгружать драйверы устройств или другой код в режиме ядра. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что не позволяет системе использовать данные в виртуальную память на диске. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут указывать параметры аудита доступа к объекту для отдельных ресурсов, таких как файлы, объекты Active Directory и ключи реестра. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут выполнять задачи технического обслуживания на томе, например удаленное дефрагментирование. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, кто может изменять значения среды прошивки. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи пользователей могут изменять метку целостности объектов, таких как файлы, ключи реестра или процессы, которыми владеют другие пользователи. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для мониторинга производительности системных процессов. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут отключить компьютер из удаленного расположения в сети. Неправильное использование этого права пользователя может привести к отказу в обслуживании. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут обходить разрешения файлов, каталогов, реестров и других постоянных объектов при восстановлении архивных файлов и каталогов, а также определяет, какие пользователи могут установить любой допустимый принцип безопасности в качестве владельца объекта. Поддерживаются только состояния NotConfigured и Allowed.|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут взять на себя право собственности на любой защищаемый объект в системе, включая объекты Active Directory, файлы и папки, принтеры, ключи реестра, процессы и потоки. Поддерживаются только состояния NotConfigured и Allowed.|
|xboxServicesEnableXboxGameSaveTask|Логическое|Этот параметр определяет, включено ли сохранение игры xbox (1) или отключено (0).|
|xboxServicesAccessoryManagementServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска службы управления аксессуарами автоматическим (2), ручным (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveAuthManagerServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска службы Live Auth Manager автоматическим (2), ручным (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveGameSaveServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска службы сохранения Live Game автоматическим (2), ручным (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveNetworkingServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), ручным (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|localSecurityOptionsBlockMicrosoftAccounts|Логическое|Запретить пользователям добавлять на этот компьютер новые учетные записи Майкрософт.|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Логическое|Включить локальные учетные записи, которые не защищены паролем, для входа из других местоположений, кроме физического устройства. Включено значение по умолчанию|
|localSecurityOptionsDisableAdministratorAccount|Логическое|Определяет, включена или отключена учетная запись локального администратора.|
|localSecurityOptionsAdministratorAccountName|String|Определите другое имя учетной записи, связанное с идентификатором безопасности (SID) для учетной записи "Администратор".|
|localSecurityOptionsDisableGuestAccount|Логическое|Определяет, включена или отключена учетная запись гостевой.|
|localSecurityOptionsGuestAccountName|String|Определите другое имя учетной записи, связанное с идентификатором безопасности (SID) для учетной записи "Гость".|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Логическое|Запретить отсоединовку портативного компьютера без входа.|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Логическое|Ограничить установку драйверов принтера в рамках подключения к общему принтеру только администраторам.|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Логическое|Включение этого параметра позволяет только в интерактивном режиме войти в систему пользователю, чтобы получить доступ к CD-ROM-носителю.|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|Определите, кому разрешено форматирование и удаление съемных носители NTFS. Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsMachineInactivityLimit|Int32|Определите максимальные минуты бездействия на экране входа на интерактивном рабочем столе до тех пор, пока не будет работать замотивник экрана. Допустимые значения от 0 до 9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|Определите максимальные минуты бездействия на экране входа на интерактивном рабочем столе до тех пор, пока не будет работать замотивник экрана. Допустимые значения от 0 до 9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|Логический|Перед входом в систему необходимо нажать на CTRL+ALT+DEL.|
|localSecurityOptionsHideLastSignedInUser|Логическое|Не отображать имя пользователя последнего человека, который вписался на этом устройстве.|
|localSecurityOptionsHideUsernameAtSignIn|Логическое|Не отображать имя пользователя пользователя, вписавшись на это устройство после входа учетных данных и до отображения рабочего стола устройства.|
|localSecurityOptionsLogOnMessageTitle|String|Установите название сообщения для пользователей, пытающихся войти в систему.|
|localSecurityOptionsLogOnMessageText|String|Установите текст сообщения для пользователей, пытающихся войти в систему.|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Логическое|Блокировать запросы на проверку подлинности PKU2U на этом устройстве для использования удостоверений в Интернете.|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Логическое|Помощник пользовательского интерфейса для подразделения LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|Изменить строку определения определения дескриптора безопасности по умолчанию, чтобы разрешить пользователям и группам делать удаленные вызовы в SAM.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Этот параметр безопасности позволяет клиенту требовать согласования 128-битного шифрования и/или безопасности сеанса NTLMv2. Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Этот параметр безопасности позволяет серверу требовать согласования 128-битного шифрования и/или безопасности сеанса NTLMv2. Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|Этот параметр безопасности определяет, какой протокол проверки подлинности вызовов и ответов используется для сетевых логотипов. Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.|
|lanManagerWorkstationDisableInsecureGuestLogons|Логическое|Если включено, клиент SMB позволит использовать небезопасные гостевых логотипы. Если он не настроен, клиент SMB отклоняет небезопасные гостевых логотипы.|
|localSecurityOptionsClearVirtualMemoryPageFile|Логическое|Этот параметр безопасности определяет, очищается ли виртуальная страница памяти при отключении системы.|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Логическое|Этот параметр безопасности определяет, можно ли отключить компьютер без необходимости входа в Windows.|
|localSecurityOptionsAllowUIAccessApplicationElevation|Логическое|Разрешить приложениям UIAccess подсказок для повышения без использования безопасного рабочего стола.|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Логическое|Виртуализация сбоев записи файлов и реестра для каждого пользователя|
|localSecurityOptionsOnlyElevateSignedExecutables|Логическое|Принудительное выполнение проверки пути сертификации PKI для заданного исполняемого файла до разрешения на запуск.|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|Определите поведение запроса на повышение для администраторов в режиме утверждения администратора. Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|Определите поведение запроса высоты для стандартных пользователей. Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Логическое|Включить все запросы на повышение, чтобы перейти на рабочий стол интерактивного пользователя, а не на безопасный рабочий стол. Используются оперативные параметры политики поведения для администраторов и стандартных пользователей.|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Логическое|Установки приложений, требующие повышенных привилегий, будут подсказок для учетных данных администратора. Включено значение по умолчанию|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Логическое|Разрешить приложениям UIAccess подсказок для повышения без использования безопасного рабочего стола. Включено значение по умолчанию|
|localSecurityOptionsUseAdminApprovalMode|Логическое|Определяет, использует ли встроенная учетная запись администратора режим утверждения администратора или запускает все приложения с полными привилегиями администратора. Включено значение по умолчанию|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Логическое|Определите, включен ли режим утверждения администрирования и все параметры политики UAC по умолчанию|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|Настройка пользовательских сведений, отображаемых при блокировке сеанса. Если они не настроены, отображается имя пользователя, домен и имя пользователя. Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|Настройка пользовательских сведений, отображаемых при блокировке сеанса. Если они не настроены, отображается имя пользователя, домен и имя пользователя. Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Логический|Этот параметр безопасности определяет, пытается ли клиент SMB договориться о подписании пакета SMB.|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Логическое|Этот параметр безопасности определяет, требуется ли подписывать пакет клиентского компонента SMB.|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Логическое|Если этот параметр безопасности включен, перенаправлению Блока сообщений сервера (SMB) разрешается отправлять простые пароли на серверы SMB, не включаемые в Microsoft, которые не поддерживают шифрование паролей во время проверки подлинности.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Логическое|Этот параметр безопасности определяет, требуется ли подписание пакета компонентом сервера SMB.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Логическое|Этот параметр безопасности определяет, будет ли SMB-сервер согласовывать подписание пакетов SMB с клиентами, которые его запрашивают.|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Логическое|По умолчанию этот параметр безопасности ограничивает анонимный доступ к акциям и трубам к настройкам именных труб, к которые можно получить анонимный доступ, а также к акциям, к которые можно получить анонимный доступ.|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Логическое|Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены для анонимных подключений к компьютеру.|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Логическое|Этот параметр безопасности определяет, разрешает ли анонимным пользователям выполнять определенные действия, такие как список имен учетных записей домена и сетевых акций.|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Логическое|Этот параметр безопасности определяет, сохраняется ли при следующем изменении пароля значение hash-значения lan Manager (LM) для нового пароля. Он не хранится по умолчанию.|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);|Этот параметр безопасности определяет, что происходит, когда смарт-карта для зарегистрированного пользователя удаляется из чтения смарт-карт. Возможные значения: `noAction`, `lockWorkstation`, `forceLogoff`, `disconnectRemoteDesktopSession`.|
|defenderSecurityCenterDisableAppBrowserUI|Логический|Используется для отключения отображения области защиты приложения и браузера.|
|defenderSecurityCenterDisableFamilyUI|Логическое|Используется для отключения отображения области семейных параметров.|
|defenderSecurityCenterDisableHealthUI|Логическое|Используется для отключения отображения производительности устройства и области работоспособности.|
|defenderSecurityCenterDisableNetworkUI|Логическое|Используется для отключения отображения брандмауэра и области защиты сети.|
|defenderSecurityCenterDisableVirusUI|Логическое|Используется для отключения отображения области защиты от вирусов и угроз.|
|defenderSecurityCenterDisableAccountUI|Логическое|Используется для отключения отображения области защиты учетной записи.|
|defenderSecurityCenterDisableClearTpmUI|Логическое|Используется для отключения отображения кнопки Clear TPM.|
|defenderSecurityCenterDisableHardwareUI|Логическое|Используется для отключения отображения области защиты оборудования.|
|defenderSecurityCenterDisableNotificationAreaUI|Логическое|Используется для отключения отображения управления областью уведомлений. Чтобы этот параметр вступил в силу, пользователю необходимо либо выйти, либо войти, либо перезагрустить компьютер.|
|defenderSecurityCenterDisableRansomwareUI|Логическое|Используется для отключения отображения области защиты вымогателей. |
|defenderSecurityCenterDisableSecureBootUI|Логическое|Используется для отключения отображения безопасной области загрузки под безопасностью устройства.|
|defenderSecurityCenterDisableTroubleshootingUI|Логическое|Используется для отключения отображения устранения неполадок процесса безопасности в области безопасности устройства.|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|Логическое|Используется для отключения отображения обновления прошивки TPM при обнаружении уязвимого прошивки.|
|defenderSecurityCenterOrganizationDisplayName|String|Имя компании, отображаемая пользователям.|
|defenderSecurityCenterHelpEmail|String|Адрес электронной почты, отображаемой пользователям.|
|defenderSecurityCenterHelpPhone|String|Номер телефона или Skype, отображаемого пользователям.|
|defenderSecurityCenterHelpURL|String|URL-адрес портала справки, отображаемый пользователями.|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|Уведомления, отображаемые из отображаемой области приложения. Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|Настройка отображения контактных данных ИТ для конечных пользователей. Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.|
|windowsDefenderTamperProtection|[windowsDefenderTamperProtectionOptions](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|Настройка параметров защитника Windows TamperProtection. Возможные значения: `notConfigured`, `enable`, `disable`.|
|firewallBlockStatefulFTP|Boolean|Блокирует FTP-подключения к устройству с отслеживанием состояния.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно. По истечении этого срока сопоставления безопасности перестают действовать и удаляются. Допустимые значения: от 300 до 3600|
|firewallPreSharedKeyEncodingMethod|[брандмауэрPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|Выберите кодику предварительного ключа, которая будет использоваться. Возможные значения: `deviceDefault`, `none`, `utF8`.|
|firewallIPSecExemptionsNone|Логическое|Настройка исключений IPSec без исключений|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.|
|firewallIPSecExemptionsAllowICMP|Boolean|Настраивает исключения IPSec для разрешения ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.|
|firewallIPSecExemptionsAllowDHCP|Boolean|Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6|
|firewallCertificateRevocationListCheckMethod|[брандмауэрCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|Укажите, как будет применяться список отзывов сертификатов. Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Boolean|Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|Настраивает, как следует применять очереди пакетов в сценарии шлюза туннеля. Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для доменных сетей|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для общедоступных сетей|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для частных сетей|
|defenderAdobeReaderLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение Adobe Reader при создании детских процессов. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderAttackSurfaceReductionExcludedPaths|Коллекция String|Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение Office приложений, впрыскивающихся в другие процессы. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение Office приложений, впрыскивающихся в другие процессы. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeCommunicationAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение Office, включая Microsoft Outlook, от создания детских процессов. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение Office приложений/макрос, создаваемых или запускаемых исполняемого контента. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение Office приложений/макрос, создаваемых или запускаемых исполняемого контента. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение Office запуска детских процессов. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение Office запуска детских процессов. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение импорта Win32 из кода Macro в Office. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение импорта Win32 из кода Macro в Office. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение запутываемого кода js/vbs/ps/macro. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение запутываемого кода js/vbs/ps/macro. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение js/vbs для выполнения полезной нагрузки, скачанных из Интернета. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение js/vbs для выполнения полезной нагрузки, скачанных из Интернета. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее, разрешен ли кража учетных данных из Windows подсистемы местного органа безопасности. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее отклик на создание процессов, происходящих из команд PSExec и WMI. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее отклик на создание процессов, происходящих из команд PSExec и WMI. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее ответ на ненарушимые и неподписаные процессы, которые запускают из USB. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее ответ на ненарушимые и неподписаные процессы, которые запускают из USB. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее ответ на исполняемые, которые не соответствуют критериям распространенности, возраста или доверенного списка. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее ответ на исполняемые, которые не соответствуют критериям распространенности, возраста или доверенного списка. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее, что выполнение исполняемого контента (exe, dll, ps, js, vbs и т.д.) должно быть отброшено из электронной почты (веб-почта/почтовый клиент). Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее, что выполнение исполняемого контента (exe, dll, ps, js, vbs и т.д.) должно быть отброшено из электронной почты (веб-почта/почтовый клиент). Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее использование передовой защиты от программ-вымогателей. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|Значение, указывающее поведение защищенных папок. Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.|
|defenderGuardedFoldersAllowedAppPaths|Коллекция String|Список путей к файлам EXE, которым разрешен доступ к защищенным папкам|
|defenderAdditionalGuardedFolders|Коллекция String|Список путей к папкам, которые следует добавить в список защищенных папок|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение NetworkProtection. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderExploitProtectionXml|Binary|XML-файл с информацией о защите от эксплойтов.|
|defenderExploitProtectionXmlFileName|String|Имя файла, из которого получено свойство DefenderExploitProtectionXml.|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.|
|defenderBlockPersistenceThroughWmiType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение сохраняемого блока с помощью подписки на события WMI. Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|Позволяет администратору выбирать разрешенные типы приложений для устройств. Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|Включай учетную защиту, когда включен уровень безопасности платформы с безопасностью безопасной загрузки и безопасностью на основе виртуализации. Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.|
|deviceGuardEnableVirtualizationBasedSecurity|Логическое|Включает безопасность на основе виртуализации (VBS).|
|deviceGuardEnableSecureBootWithDMA|Логическое|Это свойство будет обесценилось в мае 2019 г. и будет заменено свойством DeviceGuardSecureBootWithDMA. Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.|
|deviceGuardSecureBootWithDMA|[secureBootWithDMAType](../resources/intune-deviceconfig-securebootwithdmatype.md)|Указывает, включен ли уровень безопасности платформы при следующей перезагрузке. Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.|
|deviceGuardLaunchSystemGuard|[включить](../resources/intune-shared-enablement.md)|Позволяет ИТ-администратору настроить запуск System Guard. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|smartScreenEnableInShell|Boolean|Позволяет ИТ-администраторам настраивать SmartScreen для Windows.|
|smartScreenBlockOverrideForFiles|Boolean|Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.|
|applicationGuardEnabled|Boolean|Включение Application Guard в Защитнике Windows|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|Включить Application Guard в Защитнике Windows для новых Windows сборки. Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|Блокировка буфера обмена для передачи файла изображений, текстового файла или ни одного из них. Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolean|Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.|
|applicationGuardAllowPersistence|Boolean|Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).|
|applicationGuardForceAuditing|Boolean|Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена. Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolean|Позволяет разрешить печать в PDF из контейнера.|
|applicationGuardAllowPrintToXPS|Boolean|Позволяет разрешить печать в XPS из контейнера.|
|applicationGuardAllowPrintToLocalPrinters|Boolean|Позволяет разрешить печать на локальных принтерах из контейнера.|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|Позволяет разрешить печать на сетевых принтерах из контейнера.|
|applicationGuardAllowVirtualGPU|Логическое|Разрешить охраннику приложения использовать виртуальный GPU|
|applicationGuardAllowFileSaveOnHost|Логическое|Разрешить пользователям скачивать файлы из Edge в контейнере охраны приложений и сохранять их в файловой системе хост|
|applicationGuardAllowCameraMicrophoneRedirection|Логическое|Получает или задает, могут ли приложения внутри Application Guard в Microsoft Defender получить доступ к камере и микрофону устройства.|
|applicationGuardCertificateThumbprints|Коллекция String|Позволяет совместно использовать корневые сертификаты определенного уровня устройств с Application Guard в Microsoft Defender контейнером.|
|bitLockerAllowStandardUserEncryption|Логическое|Позволяет администратору разрешить стандартным пользователям включить encrpytion во время azure AD Join.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|Позволяет администратору требовать включения шифрования с помощью BitLocker. Эта политика действительна только для мобильных устройств.|
|bitLockerEncryptDevice|Boolean|Позволяет администратору требовать включения шифрования с помощью BitLocker.|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|Политика привода системы BitLocker.|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);|Политика фиксированного диска BitLocker.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|Политика BitLocker в отношении съемных дисков.|
|bitLockerRecoveryPasswordRotation|[bitLockerRecoveryPasswordRotationType](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|Этот параметр инициирует вращение пароля на основе клиента после восстановления диска ОС (с помощью bootmgr или WinRE). Возможные значения: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.|
|defenderDisableScanArchiveFiles|Логическое|Позволяет или не разрешает сканирование архивов.|
|defenderAllowScanArchiveFiles|Логическое|Позволяет или не разрешает сканирование архивов.|
|defenderDisableBehaviorMonitoring|Логическое|Позволяет или не разрешает Защитник Windows функции мониторинга поведения.|
|defenderAllowBehaviorMonitoring|Boolean|Позволяет или не разрешает Защитник Windows функции мониторинга поведения.|
|defenderDisableCloudProtection|Логический|Чтобы лучше защитить компьютер, Защитник Windows отправляет в Корпорацию Майкрософт сведения о любых проблемах, которые он находит. Корпорация Майкрософт проанализирует эту информацию, узнает больше о проблемах, затрагивающих вас и других клиентов, и предложит улучшенные решения.|
|defenderAllowCloudProtection|Boolean|Чтобы лучше защитить компьютер, Защитник Windows отправляет в Корпорацию Майкрософт сведения о любых проблемах, которые он находит. Корпорация Майкрософт проанализирует эту информацию, узнает больше о проблемах, затрагивающих вас и других клиентов, и предложит улучшенные решения.|
|defenderEnableScanIncomingMail|Логический|Позволяет или не разрешает сканирование электронной почты.|
|defenderEnableScanMappedNetworkDrivesDuringFullScan|Boolean|Позволяет или не разрешает полное сканирование картографифицированных сетевых дисков.|
|defenderDisableScanRemovableDrivesDuringFullScan|Логическое|Позволяет или отстраняет полное сканирование съемных дисков. Во время быстрого сканирования съемные диски могут по-прежнему проверяться.|
|defenderAllowScanRemovableDrivesDuringFullScan|Логическое|Позволяет или отстраняет полное сканирование съемных дисков. Во время быстрого сканирования съемные диски могут по-прежнему проверяться.|
|defenderDisableScanDownloads|Логическое|Позволяет или не разрешает Защитник Windows IOAVP Protection.|
|defenderAllowScanDownloads|Логическое|Позволяет или не разрешает Защитник Windows IOAVP Protection.|
|defenderDisableIntrusionPreventionSystem|Логическое|Позволяет или не разрешает Защитник Windows функции предотвращения вторжений.|
|defenderAllowIntrusionPreventionSystem|Логическое|Позволяет или не разрешает Защитник Windows функции предотвращения вторжений.|
|defenderDisableOnAccessProtection|Логическое|Позволяет или не разрешает Защитник Windows функции защиты доступа.|
|defenderAllowOnAccessProtection|Логическое|Позволяет или не разрешает Защитник Windows функции защиты доступа.|
|defenderDisableRealTimeMonitoring|Логический|Позволяет или не разрешает Защитник Windows функции мониторинга реального времени.|
|defenderAllowRealTimeMonitoring|Логический|Позволяет или не разрешает Защитник Windows функции мониторинга реального времени.|
|defenderDisableScanNetworkFiles|Логический|Позволяет или не разрешает сканирование сетевых файлов.|
|defenderAllowScanNetworkFiles|Логическое|Позволяет или не разрешает сканирование сетевых файлов.|
|defenderDisableScanScriptsLoadedInInternetExplorer|Логическое|Позволяет или не разрешает Защитник Windows скриптов.|
|defenderAllowScanScriptsLoadedInInternetExplorer|Логическое|Позволяет или не разрешает Защитник Windows скриптов.|
|defenderBlockEndUserAccess|Boolean|Позволяет или не разрешает пользователю доступ к пользовательскому Защитник Windows пользовательскому интерфейсу. Если они будут отложены, Защитник Windows уведомления будут также подавлены.|
|defenderAllowEndUserAccess|Логическое|Позволяет или не разрешает пользователю доступ к пользовательскому Защитник Windows пользовательскому интерфейсу. Если они будут отложены, Защитник Windows уведомления будут также подавлены.|
|defenderScanMaxCpuPercentage|Int32|Представляет средний коэффициент нагрузки ЦП для Защитник Windows проверки (в процентах). Значение по умолчанию равно 50. Допустимые значения: от 0 до 100|
|defenderCheckForSignaturesBeforeRunningScan|Логический|Этот параметр политики позволяет управлять проверкой новых определений вирусов и программ-шпионов перед запуском сканирования.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Добавлена Windows 10 версии 1709. Этот параметр политики определяет, насколько антивирусная программа  будут блокировать и сканировать подозрительные файлы. Тип значения является integer. Для этой функции требуется включить параметр "Присоединиться к Microsoft MAPS". Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeoutInSeconds|Int32|Добавлена Windows 10 версии 1709. Эта функция позволяет антивирусная программа  подозрительный файл на срок до 60 секунд и сканировать его в облаке, чтобы убедиться, что он является безопасным. Тип значения является наборным, диапазон — 0 — 50. Эта функция зависит от трех других параметров MAPS, которые необходимо включить: "Настройка функции "Блок с первого взгляда"; " Присоединяйтесь к Microsoft MAPS"; "Отправка образцов файлов при необходимости дальнейшего анализа". Допустимые значения: от 0 до 50.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Период времени (в днях), когда элементы карантина будут храниться в системе. Допустимые значения: от 0 до 90.|
|defenderDisableCatchupFullScan|Логический|Этот параметр политики позволяет настроить проверки наверстать упущенное для запланированных полных сканов. Проверка наверстать упущенное — это проверка, которая инициируется из-за пропущенного регулярно запланированного сканирования. Обычно эти запланированные проверки пропускаются из-за отключения компьютера в запланированное время.|
|defenderDisableCatchupQuickScan|Логическое|Этот параметр политики позволяет настроить проверки наверстать упущенное для запланированных быстрых сканирований. Проверка наверстать упущенное — это проверка, которая инициируется из-за пропущенного регулярно запланированного сканирования. Обычно эти запланированные проверки пропускаются из-за отключения компьютера в запланированное время.|
|defenderEnableLowCpuPriority|Логическое|Этот параметр политики позволяет включить или отключить низкий приоритет ЦП для запланированных сканов.|
|defenderFileExtensionsToExclude|Коллекция String|Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderFilesAndFoldersToExclude|Коллекция String|Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderProcessesToExclude|Коллекция String|Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderPotentiallyUnwantedAppAction|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Добавлено в Windows 10 версии 1607. Указывает уровень обнаружения для потенциально нежелательных приложений (PUAs). Защитник Windows оповещает вас о скачиве потенциально нежелательного программного обеспечения или попытках установить себя на компьютере. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderScanDirection|[defenderRealtimeScanDirection](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|Контролирует, какие наборы файлов следует отслеживать. Возможные значения: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Выбирает, следует ли выполнять быстрое сканирование или полное сканирование. Возможные значения: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledQuickScanTime|TimeOfDay|Выбирает время суток, когда Защитник Windows быстрое сканирование. Например, значение 0=12:00AM, значение 60=1:00AM, значение 120=2:00 и так далее, до значения 1380=11:00PM. Значение по умолчанию — 120|
|defenderScheduledScanDay|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Выбирает день запуска Защитник Windows проверки. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderScheduledScanTime|TimeOfDay|Выбирает время суток, в которое должна Защитник Windows проверка.|
|defenderSignatureUpdateIntervalInHours|Int32|Указывает интервал (в часах), который будет использоваться для проверки подписей, поэтому вместо использования ScheduleDay и ScheduleTime проверка новых подписей будет задана в соответствии с интервалом. Допустимые значения: от 0 до 24.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);|Проверка уровня согласия пользователя в Защитник Windows для отправки данных. Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Позволяет администратору указать допустимые уровни серьезности угрозы и соответствующий ИД действий по умолчанию.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|

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




