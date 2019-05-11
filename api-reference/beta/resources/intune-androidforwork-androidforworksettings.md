---
title: Тип ресурса androidForWorkSettings
description: Параметры Android For Work.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66996681929c55d44ef94fdcf88d292ac34021a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950587"
---
# <a name="androidforworksettings-resource-type"></a>Тип ресурса androidForWorkSettings

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры Android For Work.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md);|Чтение свойств и связей объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Обновление объекта androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Действие requestSignupUrl](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|String|Пока не задокументировано.|
|[completeSignup action](../api/intune-androidforwork-androidforworksettings-completesignup.md)|Нет|Пока не задокументировано|
|[Действие syncApps](../api/intune-androidforwork-androidforworksettings-syncapps.md)|Нет|Пока не задокументировано|
|[Действие unbind](../api/intune-androidforwork-androidforworksettings-unbind.md)|Нет|Пока не задокументировано|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор параметров Android for Work|
|bindStatus|[Андроидфорворкбиндстатус](../resources/intune-androidforwork-androidforworkbindstatus.md)|Состояние связывания клиента с помощью API Google EMM. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|[Андроидфорворксинкстатус](../resources/intune-androidforwork-androidforworksyncstatus.md)|Последний результат синхронизации приложений. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|Строка|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Имя организации, используемое при входящей миграции Android for Work|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения параметров Android for Work|
|enrollmentTarget|[Андроидфорворкенроллменттаржет](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Указывает, какие пользователи могут регистрировать устройства в Android для управления рабочими устройствами. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|
|Девицеовнерманажементенаблед|Логический|Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.|

## <a name="relationships"></a>Связи
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




