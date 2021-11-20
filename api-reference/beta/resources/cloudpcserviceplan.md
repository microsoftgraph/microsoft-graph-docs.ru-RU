---
title: тип ресурса cloudPcServicePlan
description: Представляет план Windows 365, настроенный для облачного КОМПЬЮТЕРА.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 281bfdbaefde3b58b8bb9c0367d92d7dfc0bebb3
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123953"
---
# <a name="cloudpcserviceplan-resource-type"></a>тип ресурса cloudPcServicePlan

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет план Windows 365, настроенный для облачного КОМПЬЮТЕРА.

Примеры доступных планов обслуживания см. в Windows [365 сравните планы и цены.](https://www.microsoft.com/windows-365/business/compare-plans-pricing) В настоящее время Graph API Microsoft доступен для Windows 365 Enterprise.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список servicePlans](../api/virtualendpoint-list-serviceplans.md)|[коллекция cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Список доступных в настоящее время планов служб, которые организация может приобрести для облачных компьютеров.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя плана службы. Только для чтения.|
|id|String|Уникальный идентификатор для плана службы. Только для чтения.|
|ramInGB|Int32|Размер оперативной памяти в ГБ. Только для чтения.|
|storageInGB|Int32|Размер диска ОС в ГБ. Только для чтения.|
|type|[cloudPcServicePlanType](#cloudpcserviceplantype-values)|Тип плана обслуживания. Возможные значения: `enterprise`, `business`, `unknownFutureValue`. Только для чтения.|
|userProfileInGB|Int32|Размер диска профиля пользователя в ГБ. Только для чтения.|
|vCpuCount|Int32|Число vCPUs. Только для чтения.|

### <a name="cloudpcserviceplantype-values"></a>значения cloudPcServicePlanType

|Member|Описание|
|:---|:---|
|корпоративный|Enterprise тип плана обслуживания для корпоративных клиентов.|
|бизнес|Тип плана бизнес-служб для клиентов очень малого бизнеса (VSB).|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcServicePlan",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcServicePlan",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "vCpuCount": "Int32",
  "ramInGB": "Int32",
  "storageInGB": "Int32",
  "userProfileInGB": "Int32"
}
```
