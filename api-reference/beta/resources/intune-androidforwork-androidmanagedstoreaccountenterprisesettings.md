---
title: Тип ресурса ресурса androidmanagedstoreaccountenterprisesettings
description: Корпоративные параметры для учетной записи управляемого хранилища Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6f640882f5b1041a37ec267d5f9726715afaa6c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950615"
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
|[completeSignup action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|Нет|Пока не задокументировано|
|[Действие syncApps](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|Нет|Пока не задокументировано|
|[Действие unbind](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|Нет|Пока не задокументировано|
|[Действие createGooglePlayWebToken](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|Строка|Создает веб-токен, используемый в встраиваемом компоненте.|
|[Действие setAndroidDeviceOwnerFullyManagedEnrollmentState](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|Нет|Задает для ресурса androidmanagedstoreaccountenterprisesettings Андроиддевицеовнерфуллиманажеденроллментенаблед заданное значение.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор корпоративных параметров учетной записи магазина Android|
|bindStatus|[Андроидманажедстореаккаунтбиндстатус](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Состояние связывания клиента с помощью API Google EMM. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|[Андроидманажедстореаккаунтаппсинкстатус](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|Последний результат синхронизации приложений. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|Строка|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Название организации, используемое при входящей миграции для Android Enterprise|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения корпоративных параметров для Android|
|enrollmentTarget|[Андроидманажедстореаккаунтенроллменттаржет](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Указывает, какие пользователи могут регистрировать устройства в управлении устройствами Android Enterprise. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|
|Девицеовнерманажементенаблед|Логический|Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.|
|Компаникодес|Коллекция [андроиденроллменткомпаникоде](../resources/intune-androidforwork-androidenrollmentcompanycode.md)|Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings|
|Андроиддевицеовнерфуллиманажеденроллментенаблед|Логический|Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings|

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




