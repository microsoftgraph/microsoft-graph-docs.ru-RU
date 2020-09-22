---
title: Тип ресурса androidForWorkSettings
description: Параметры Android For Work.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef0452ea29b6966f24778662a429bb1534c8068f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052857"
---
# <a name="androidforworksettings-resource-type"></a>Тип ресурса androidForWorkSettings

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры Android For Work.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Чтение свойств и связей объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Обновление объекта androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Действие requestSignupUrl](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|String|Пока не задокументировано.|
|[completeSignup action](../api/intune-androidforwork-androidforworksettings-completesignup.md)|Нет|Н/Д|
|[Действие syncApps](../api/intune-androidforwork-androidforworksettings-syncapps.md)|Нет|Н/Д|
|[Действие unbind](../api/intune-androidforwork-androidforworksettings-unbind.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор параметров Android for Work|
|bindStatus|[андроидфорворкбиндстатус](../resources/intune-androidforwork-androidforworkbindstatus.md)|Состояние связывания клиента с помощью API Google EMM. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|[андроидфорворксинкстатус](../resources/intune-androidforwork-androidforworksyncstatus.md)|Последний результат синхронизации приложений. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Имя организации, используемое при входящей миграции Android for Work|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения параметров Android for Work|
|enrollmentTarget|[андроидфорворкенроллменттаржет](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Указывает, какие пользователи могут регистрировать устройства в Android для управления рабочими устройствами. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|
|девицеовнерманажементенаблед|Boolean|Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.|

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






