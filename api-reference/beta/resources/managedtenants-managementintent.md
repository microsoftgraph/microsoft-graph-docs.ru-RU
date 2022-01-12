---
title: тип ресурсов managementIntent
description: Представляет метаданные для базового плана и какие шаблоны управления включены.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: c3e4954e34768b711f621efe98b00eda5baae1d9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791933"
---
# <a name="managementintent-resource-type"></a>тип ресурсов managementIntent

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метаданные для базового плана и какие шаблоны управления включены.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Управление спискамиИнтенты](../api/managedtenants-managedtenant-list-managementintents.md)|[коллекция microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|Получите список объектов [managementIntent](../resources/managedtenants-managementintent.md) и их свойств.|
|[Get managementIntent](../api/managedtenants-managementintent-get.md)|[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|Ознакомьтесь с свойствами и отношениями объекта [managementIntent.](../resources/managedtenants-managementintent.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя отображения для намерения управления. Необязательно. Только для чтения.|
|id|String|Уникальный идентификатор для намерения управления. Обязательное. Только для чтения.|
|isGlobal|Логический|Флаг, указывающий, является ли намерение управления глобальным. Обязательный. Только для чтения.|
|managementTemplates|[коллекция microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md)|Коллекция шаблонов управления, связанных с намерением управления. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementIntent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "isGlobal": "Boolean",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
