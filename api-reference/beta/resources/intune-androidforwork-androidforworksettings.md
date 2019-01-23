---
title: Тип ресурса androidForWorkSettings
description: Параметры Android For Work.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c1125890ad05eb00a05f19bb765df6122a10ce7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421965"
---
# <a name="androidforworksettings-resource-type"></a>Тип ресурса androidForWorkSettings

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры Android For Work.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Чтение свойств и связей объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Обновление объекта androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Действие requestSignupUrl](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|String|Н/Д|
|[completeSignup action](../api/intune-androidforwork-androidforworksettings-completesignup.md)|Нет|Н/Д|
|[Действие syncApps](../api/intune-androidforwork-androidforworksettings-syncapps.md)|Нет|Н/Д|
|[Действие unbind](../api/intune-androidforwork-androidforworksettings-unbind.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор параметров Android for Work|
|bindStatus|[androidForWorkBindStatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|Привязка состояния клиента с помощью API EMM Google. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|[androidForWorkSyncStatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|Результат последней синхронизации приложения. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Имя организации, используемое при входящей миграции Android for Work|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения параметров Android for Work|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Указывает пользователей, которые можно зарегистрировать устройств в Android для управления работой устройства. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|
|deviceOwnerManagementEnabled|Логический|Указывает, если эта учетная запись flighting для Android владелец управление устройствами с CloudDPC.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
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
  "deviceOwnerManagementEnabled": true
}
```




