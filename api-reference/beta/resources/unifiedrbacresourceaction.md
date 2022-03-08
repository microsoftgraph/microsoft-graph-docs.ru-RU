---
title: тип ресурса unifiedRbacResourceAction
description: Представляет операцию, которую разрешено выполнять уполномоченной основной.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4407c12d18576c6a6ad560588381bc7abd2b4855
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339410"
---
# <a name="unifiedrbacresourceaction-resource-type"></a>тип ресурса unifiedRbacResourceAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет операцию, которую разрешено выполнять уполномоченной основной.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список объединенныхRbacResourceActions](../api/unifiedrbacresourcenamespace-list-resourceactions.md)|[коллекция unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|Получите список [унифицированных объектовRbacResourceAction](../resources/unifiedrbacresourceaction.md) и их свойств.|
|[Get unifiedRbacResourceAction](../api/unifiedrbacresourceaction-get.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|Ознакомьтесь с свойствами и отношениями единого [объектаRbacResourceAction](../resources/unifiedrbacresourceaction.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionVerb|Строка|HTTP-метод для действия, например `DELETE`, `GET`, `PATCH`, , , `POST`или `PUT``null`. `$filter` Поддерживает (`eq`), но не для `null` значений. |
|description|Строка|Описание действия. Поддерживает `$filter` (`eq`). |
|id|String|Уникальный идентификатор для действия в пространстве имен ресурсов, например `microsoft.insights-programs-update-patch`. Не может включать символ slash (`/`). Случай нечувствительный. Обязательный элемент. Поддерживает `$filter` (`eq`). |
|name|String|Имя действия в пространстве имен ресурсов, например `microsoft.insights/programs/update`. Может включать символ slash (`/`). Случай нечувствительный. Обязательный элемент. Поддерживает `$filter` (`eq`). |
|resourceScopeId|String|Не реализовано.|

## <a name="relationships"></a>Связи

Отсутствуют.

<!-- The resourceScope relationship hasn't been implemented but is in the public schema. To unhide this and its related entities and methods once it's implemented.
|Relationship|Type|Description|
|:---|:---|:---|
|resourceScope| [unifiedRbacResourceScope](unifiedrbacresourcescope.md) |Not implemented.|
-->

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRbacResourceAction",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceAction",
  "id": "String (identifier)",
  "actionVerb": "String",
  "description": "String",
  "name": "String",
  "resourceScopeId": "String"
}
```
