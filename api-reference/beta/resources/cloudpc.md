---
title: Тип ресурса cloudPC
description: Виртуальные рабочие столы, управляемые облаком.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 481bcae691632685cafab00a4b7e44addb1ad0cd
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706089"
---
# <a name="cloudpc-resource-type"></a>Тип ресурса cloudPC

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет управляемый облаком виртуальный рабочий стол.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)|
|[Get cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Чтение свойств и связей объекта [cloudPC.](../resources/cloudpc.md)|
|[Reprovision](../api/cloudpc-reprovision.md)|Нет|Повторное создание объекта [cloudPC.](../resources/cloudpc.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для облачного ПК. Только для чтения.|
|displayName|String|Отображаемая версия облачного компьютера.|
|imageDisplayName|String|Имя образа ОС на облачном компьютере.|
|managedDeviceId|String|ИД устройства Intune на облачном компьютере.|
|managedDeviceName|String|Имя устройства Intune облачного ПК.|
|provisioningPolicyId|String|ИД политики предоставления на облачном компьютере.|
|servicePlanId|String|ИД плана обслуживания облачного КОМПЬЮТЕРА.|
|servicePlanName|String|Имя плана обслуживания облачного ПК.|
|status|cloudPcStatus|Состояние облачного ПК. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Сведения о состоянии облачного ПК.|
|userPrincipalName|String|Имя основного пользователя (UPN) пользователя, назначенного облачному компьютеру.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения облачного ПК. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPC",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPC",
  "id": "String (identifier)",
  "displayName": "String",
  "imageDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```
