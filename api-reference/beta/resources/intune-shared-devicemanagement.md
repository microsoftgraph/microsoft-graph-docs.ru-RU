---
title: Тип ресурса deviceManagement
description: 'Ресурс deviceManagement представляет контейнер, содержимое которого различаться в зависимости от рабочего процесса, включая:  '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2f4348da007a3d69d1618151718789d1b72e3e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961339"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс deviceManagement представляет контейнер, содержимое которого различаться в зависимости от рабочего процесса, включая:  

- Параметры Android for Work
- События аудита
- Корпоративный сроками и условиями 
- Профили организации подачи заявок
- Параметры конфигурации устройства
- Управление устройствами
- Электронные диспетчер установки (ESIM)
- Разграничения
- Уведомления
- Адаптация новых сотрудников политики, параметры и подробные сведения
- Удаленный доступ
- Партнеры удаленный помощник
- Политики управления ДОСТУПОМ на основе ролей доступа
- Партнеры управления просторам телекоммуникации
- Устранение неполадок для событий
- Защита информации Windows сводки

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-shared-devicemanagement-get.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-shared-devicemanagement-update.md)|Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|**Конфигурация устройств**|
|[Действие enableLegacyPcManagement](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|Нет|Н/Д|
|**Управление устройствами**|
|[Действие sendCustomNotificationToCompanyPortal](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|Нет|Н/Д|
|**Адаптация новых сотрудников**|
|[Функция verifyWindowsEnrollmentAutoDiscovery](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean|Н/Д|
|**Управление доступом на основе ролей (RBAC)**|
|[Функция getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Получает действующие разрешения пользователя, прошедшего проверку подлинности|
|[функция getRoleScopeTagsByIds](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) коллекции|Н/Д|
|[функция getRoleScopeTagsByResource](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) коллекции|Н/Д|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор, связанный с устройством.|
|**Конфигурация устройств**|
|intuneAccountId|Guid|Идентификатор учетной записи Intune для заданного клиента|
|legacyPcManangementEnabled|Логический|Свойство для включения не MDM управляемых прежних версий управления ПК для этой учетной записи. Это свойство доступно только для чтения.|
|maximumDepTokens|Int32|Максимальное число DEP маркеры могут каждого клиента.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|accountMoveCompletionDateTime|DateTimeOffset|Время & даты, при перемещении данные клиента между ScaleUnits строкового.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Сведения о разрешения администратора.|
|deviceProtectionOverview;|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);|Общие сведения о защите устройств.|
|managedDeviceCleanupSettings;|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);|Правила очистки устройства|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|подписки|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Подписка клиента. Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Обзор вредоносных программ для устройств windows.|
|**Адаптация новых сотрудников**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android (en), для работы**|
|androidDeviceOwnerEnrollmentProfiles|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) коллекции|Сущностей профилей регистрации Android устройства владельцем.|
|androidForWorkAppConfigurationSchemas|Коллекция [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Сущности схемы конфигурации в приложении Android for Work.|
|androidForWorkEnrollmentProfiles|Коллекция [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Сущности профиля регистрации Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Одноэлементная сущность параметров Android for Work.|
|androidManagedStoreAccountEnterpriseSettings;|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Одного Android управление хранилища сущности корпоративных параметров учетной записи.|
|androidManagedStoreAppConfigurationSchemas|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) коллекции|Объекты приложения схемы конфигурации Android предприятия.|
|**аудита;**|
|auditEvents|Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)|События аудита|
|**Условия компании**|
|termsAndConditions|Коллекция [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Условия, связанные с управлением устройствами в компании.|
|**Корпоративный подачи заявок**|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) коллекции|Профили заявок через Интернет.|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) коллекции|Импортированные удостоверений устройства Apple.|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) коллекции|Импортированные устройства удостоверений.|
|**Конфигурация устройств**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Сводка состоянии состояния входящая ATP для этой учетной записи.|
|cartToClassAssociations|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) коллекции|Корзины для ассоциации класса.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Политики соответствия устройств требованиям.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.|
|deviceCompliancePolicySettingStateSummaries|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.|
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) коллекции|Сводка по политик в состоянии конфликта для этой учетной записи.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Общие сведения о состоянии конфигурации устройства для этой учетной записи.|
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) коллекции|Нарушения ограниченных приложений для этой учетной записи.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Конфигурации устройств.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md);|Конфигурация пользователя состояние устройства сводки для этой учетной записи.|
|iosUpdateStatuses|Коллекция [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Состояния установки обновления программного обеспечения IOS для этой учетной записи.|
|ndesConnectors|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) коллекции|Коллекция соединителей Ndes для этой учетной записи.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Общие сведения о состоянии обновления программного обеспечения.|
|**Управление устройствами**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Сертификат push-уведомлений Apple|
|dataSharingConsents|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) коллекции|Согласия общего доступа к данным.|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Список обнаруженных приложений, связанных с устройством.|
|deviceManagementScripts|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) коллекции|Список сценарии управления устройств, связанных с клиента.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Обзор устройств|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Список управляемых устройств.|
|remoteActionAudits|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) коллекции|Список удаленных действие устройства аудит с клиента.|
|windowsMalwareInformation|[windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md) коллекции|Список затронутых вредоносных программ в клиентов.|
|**Регистрация**|
|depOnboardingSettings|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) коллекции|В этом коллекции нескольких DEP маркеры каждого клиента.|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) коллекции|Импортированные устройства удостоверений.|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|
|importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) коллекции|Коллекция автопилот Windows, отправка устройств.|
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) коллекции|Профили пилотного развертывания auto Windows|
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) коллекции|Удостоверения Windows автопилот устройства содержащиеся семейства сайтов.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Настройка учетных записей Windows автопилот.|
|**Внедренные диспетчера установки**|
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) коллекции|Внедренные диспетчера установки активации кода пулы, созданные с этой учетной записи.|
|**Разграничения**|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции|Управление условия, связанные с управление устройствами компании.|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции|Операторы условие управления, связанные с управление устройствами компании.|
|**Уведомления**|
|notificationMessageTemplates|Коллекция [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Шаблоны сообщений уведомления.|
|**Адаптация новых сотрудников**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|
|Объекты deviceCategory|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список категорий устройств в клиенте.|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|Объекты deviceManagementPartner|Коллекция объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Список партнеров по управлению устройствами, настроенных с помощью клиента.|
|Объекты exchangeConnector|Коллекция объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Список соединителей Exchange, настроенных с помощью клиента.|
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) коллекции|Список Exchange на Premisis политики, настроенные с клиента.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Политики, который управляет доступа с мобильных устройств к Exchange на локальном|
|Объекты mobileThreatDefenseConnector|Коллекция объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Список соединителей Mobile Threat Defense, настроенных с помощью клиента.|
|**Удаленный доступ**|
|userPfxCertificates|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) коллекции|Коллекция PFX сертификаты, связанные с пользователем.|
|**Удаленный помощник**|
|remoteAssistancePartners|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Партнеры по удаленной помощи.|
|**Управление доступом на основе ролей (RBAC)**|
|resourceOperations|Коллекция [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Операции с ресурсами.|
|roleAssignments|Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Назначения ролей.|
|roleDefinitions|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Определения ролей.|
|roleScopeTags|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) коллекции|Теги область роли.|
|**Управление расходами телекоммуникации (Командный)**|
|telecomExpenseManagementPartners|Коллекция [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Партнеры по управлению затратами на телекоммуникации.|
|**Устранение неполадок**|
|troubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для клиента.|
|**Защита информации Windows**|
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) коллекции|Фирменная символика профили, предназначенных для групп AAD Intune|
|windowsInformationProtectionAppLearningSummaries|Коллекция [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Сводки по обучению Windows Information Protection для приложений.|
|windowsInformationProtectionNetworkLearningSummaries|Коллекция [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Сводки по обучению Windows Information Protection для сетей.|


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



