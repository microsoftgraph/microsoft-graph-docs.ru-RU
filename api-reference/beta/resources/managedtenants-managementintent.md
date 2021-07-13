---
title: тип ресурсов managementIntent
description: Представляет метаданные для базового плана и какие шаблоны управления включены.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7648da23e5d49a9bd2910c2ccbde7e676a1d7cd0
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402706"
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
|id|String|Уникальный идентификатор для намерения управления. Обязательный. Только для чтения.|
|isGlobal|Boolean|Флаг, указывающий, является ли намерение управления глобальным. Обязательный. Только для чтения.|
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
