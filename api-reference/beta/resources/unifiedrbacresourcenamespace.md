---
title: тип ресурса unifiedRbacResourceNamespace
description: Представляет пространство имен области, к которой принадлежит разрешение роли.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 85c290fc07c251864507ec34de0a4d6b6027b79e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339665"
---
# <a name="unifiedrbacresourcenamespace-resource-type"></a>тип ресурса unifiedRbacResourceNamespace

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пространство имен области или службы, например Azure AD, Intune и Exchange, определяющую разрешения на роль.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список объединенных пространствRbacResourceNamespace](../api/rbacapplicationmultiple-list-resourcenamespaces.md)|[коллекция unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md)|Получите список [унифицированных объектовRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) и их свойств.|
|[Get unifiedRbacResourceNamespace](../api/unifiedrbacresourcenamespace-get.md)|[unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md)|Ознакомьтесь с свойствами и отношениями единого [объектаRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пространства имен ресурсов, определяемого разрешениями, такими как `microsoft.aad.b2c`. Обязательный элемент.|
|name|String|Имя пространства имен ресурса. Как правило, то же имя, что и свойство **id** , например `microsoft.aad.b2c`. Обязательный элемент. Поддерживает `$filter` (`eq`, `startsWith`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|resourceActions|[коллекция unifiedRbacResourceAction](unifiedrbacresourceaction.md)|Операции, которые разрешено выполнять уполномоченной основной компании.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRbacResourceNamespace",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceNamespace",
  "id": "String (identifier)",
  "name": "String"
}
```
