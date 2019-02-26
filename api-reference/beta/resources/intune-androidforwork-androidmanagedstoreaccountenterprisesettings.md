---
title: Тип ресурса ресурса androidmanagedstoreaccountenterprisesettings
description: Корпоративные параметры для учетной записи управляемого хранилища Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd6f278963bd37276b808f221d1902fd82e23a48
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159138"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>Тип ресурса ресурса androidmanagedstoreaccountenterprisesettings

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Корпоративные параметры для учетной записи управляемого хранилища Android.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение ресурса androidmanagedstoreaccountenterprisesettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Чтение свойств и связей объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .|
|[Обновление ресурса androidmanagedstoreaccountenterprisesettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Обновление свойств объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .|
|[Действие requestSignupUrl](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|Пока не задокументировано.|
|[completeSignup action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|Нет|Н/Д|
|[Действие syncApps](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|Нет|Н/Д|
|[Действие unbind](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|Нет|Н/Д|
|[Действие createGooglePlayWebToken](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|Создает веб-токен, используемый в встраиваемом компоненте.|
|[Действие setAndroidDeviceOwnerFullyManagedEnrollmentState](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|Нет|Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор корпоративных параметров учетной записи магазина Android|
|bindStatus|[Андроидманажедстореаккаунтбиндстатус](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Состояние связывания клиента с помощью API Google EMM. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|[Андроидманажедстореаккаунтаппсинкстатус](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|Последний результат синхронизации приложений. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Название организации, используемое при входящей миграции для Android Enterprise|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения корпоративных параметров для Android|
|enrollmentTarget|[Андроидманажедстореаккаунтенроллменттаржет](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Указывает, какие пользователи могут регистрировать устройства в управлении устройствами Android Enterprise. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|
|Девицеовнерманажементенаблед|Логический|Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.|
|Компаникодес|Коллекция [андроиденроллменткомпаникоде](../resources/intune-androidforwork-androidenrollmentcompanycode.md)|Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings|
|Андроиддевицеовнерфуллиманажеденроллментенаблед|Логический|Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings|

## <a name="relationships"></a>Отношения
None

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




