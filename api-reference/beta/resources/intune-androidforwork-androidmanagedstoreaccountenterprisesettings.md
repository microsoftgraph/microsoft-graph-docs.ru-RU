---
title: тип ресурса androidManagedStoreAccountEnterpriseSettings
description: Enterprise для учетной записи управляемого магазина Android.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f06f7d042977605214a286ec76ec4fd9c5ee88ca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101914"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>тип ресурса androidManagedStoreAccountEnterpriseSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Enterprise для учетной записи управляемого магазина Android.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Чтение свойств и связей [объекта AndroidManagedStoreAccountEnterpriseSettings.](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|
|[Обновление androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Обновление свойств объекта [AndroidManagedStoreAccountEnterpriseSettings.](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|
|[действие approveApps](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-approveapps.md)|Нет|Н/Д|
|[Действие requestSignupUrl](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|Пока не задокументировано.|
|[completeSignup action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|Нет|Н/Д|
|[Действие syncApps](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|Нет|Н/Д|
|[Действие unbind](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|Нет|Н/Д|
|[Действие createGooglePlayWebToken](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|Создает веб-маркер, используемый в встраивомом компоненте.|
|[Действие setAndroidDeviceOwnerFullyManagedEnrollmentState](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|Нет|Задает Значение AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор корпоративных параметров учетной записи магазина Android|
|bindStatus|[AndroidManagedStoreAccountBindStatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Связать состояние клиента с API EMM Google. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|[AndroidManagedStoreAccountAppSyncStatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|Результат синхронизации последнего приложения. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Имя организации, используемая при вовсю Enterprise|
|lastModifiedDateTime|DateTimeOffset|Время последней модификации для корпоративных параметров Android|
|enrollmentTarget|[AndroidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Указывает, какие пользователи могут записать устройства в управление Enterprise устройств. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|
|deviceOwnerManagementEnabled|Логическое|Указывает, работает ли эта учетная запись для управления владельцем android-устройств с помощью CloudDPC.|
|companyCodes|[коллекция androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)|Коды компании для AndroidManagedStoreAccountEnterpriseSettings|
|androidDeviceOwnerFullyManagedEnrollmentEnabled|Логическое|Коды компании для AndroidManagedStoreAccountEnterpriseSettings|
|managedGooglePlayInitialScopeTagIds|Коллекция объектов string|Начальные теги области для приложений MGP|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAccountEnterpriseSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "String",
      "qrCodeContent": "String",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "String",
        "value": "binary"
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true,
  "managedGooglePlayInitialScopeTagIds": [
    "String"
  ]
}
```



