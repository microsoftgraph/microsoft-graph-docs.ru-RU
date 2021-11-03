---
title: тип ресурса cloudPcServicePlan
description: Представляет определенный набор конфигураций плана обслуживания, поддерживаемый облачными компьютерами для клиента.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d2950e65ec3f90f2c7a3e55123e46c435dc805f4
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697452"
---
# <a name="cloudpcserviceplan-resource-type"></a>тип ресурса cloudPcServicePlan

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор конфигураций плана обслуживания, поддерживаемый облачными компьютерами для клиента.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список servicePlans](../api/virtualendpoint-list-serviceplans.md)|[коллекция cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Перечислить планы службы, поддерживаемые облачными компьютерами для этого клиента.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя плана службы. Только для чтения.|
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
