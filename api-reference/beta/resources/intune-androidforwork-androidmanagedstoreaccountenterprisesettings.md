---
title: Тип ресурса ресурса androidmanagedstoreaccountenterprisesettings
description: Корпоративные параметры для учетной записи управляемого хранилища Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d4a0803b766b96d957b484baa81f807f1e8f35d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013519"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>Тип ресурса ресурса androidmanagedstoreaccountenterprisesettings

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Корпоративные параметры для учетной записи управляемого хранилища Android.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение ресурса androidmanagedstoreaccountenterprisesettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Чтение свойств и связей объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .|
|[Обновление ресурса androidmanagedstoreaccountenterprisesettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Обновление свойств объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .|
|[действие Аппровеаппс](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-approveapps.md)|Нет|Н/Д|
|[Действие requestSignupUrl](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|Пока не задокументировано.|
|[completeSignup action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|Нет|Н/Д|
|[Действие syncApps](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|Нет|Н/Д|
|[Действие unbind](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|Нет|Н/Д|
|[Действие createGooglePlayWebToken](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|Создает веб-токен, используемый в встраиваемом компоненте.|
|[Действие setAndroidDeviceOwnerFullyManagedEnrollmentState](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|Нет|Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор корпоративных параметров учетной записи магазина Android|
|bindStatus|[андроидманажедстореаккаунтбиндстатус](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Состояние связывания клиента с помощью API Google EMM. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|[андроидманажедстореаккаунтаппсинкстатус](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|Последний результат синхронизации приложений. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Название организации, используемое при входящей миграции для Android Enterprise|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения корпоративных параметров для Android|
|enrollmentTarget|[андроидманажедстореаккаунтенроллменттаржет](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Указывает, какие пользователи могут регистрировать устройства в управлении устройствами Android Enterprise. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|
|девицеовнерманажементенаблед|Boolean|Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.|
|компаникодес|Коллекция [андроиденроллменткомпаникоде](../resources/intune-androidforwork-androidenrollmentcompanycode.md)|Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings|
|андроиддевицеовнерфуллиманажеденроллментенаблед|Boolean|Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings|

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
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```






