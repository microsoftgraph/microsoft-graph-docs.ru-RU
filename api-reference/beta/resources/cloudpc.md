---
title: Тип ресурса Клаудпк
description: Облачные управляемые виртуальные рабочие столы.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 95758299f87ac463bac6fdc30f7d70fb59eb6c92
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378608"
---
# <a name="cloudpc-resource-type"></a>Тип ресурса Клаудпк

Пространство имен: microsoft.graph

Представляет виртуальный рабочий стол, управляемый облаком.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Клаудпкс](../api/virtualendpoint-list-cloudpcs.md)|Коллекция [клаудпк](../resources/cloudpc.md)|Список свойств и связей объектов [клаудпк](../resources/cloudpc.md) .|
|[Получение Клаудпк](../api/cloudpc-get.md)|[клаудпк](../resources/cloudpc.md)|Чтение свойств и связей объекта [клаудпк](../resources/cloudpc.md) .|
|[Повторная подготовка](../api/cloudpc-reprovision.md)|Нет|Повторное наполнение объекта [клаудпк](../resources/cloudpc.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для облачного компьютера. Только для чтения.|
|displayName|Строка|Отображаемое имя Cloud PC.|
|имажедисплайнаме|Строка|Имя образа операционной системы, который находится на облачном компьютере.|
|манажеддевицеид|Строка|ИДЕНТИФИКАТОР устройства Intune облачного компьютера.|
|managedDeviceName|String|Имя устройства в Intune на облачном компьютере.|
|провисионингполициид|Строка|Идентификатор политики подготовки для облачного компьютера.|
|сервицепланид|Строка|ИДЕНТИФИКАТОР плана обслуживания Cloud PC.|
|сервицепланнаме|String|Имя плана обслуживания для облачного компьютера.|
|status|клаудпкстатус|Состояние облачного компьютера. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.|
|статусдетаилс|[клаудпкстатусдетаилс](../resources/cloudpcstatusdetails.md)|Сведения о состоянии облачного компьютера.|
|userPrincipalName|String|Имя участника-пользователя (UPN) пользователя, назначенное облачному компьютеру.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения в облачном ПК. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|

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
