---
title: тип ресурса tenantTag
description: Представляет тег, который может быть назначен управляемому клиенту.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e48ad25e2af3ac491c6affe4bbb4712ab45e42fc
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402652"
---
# <a name="tenanttag-resource-type"></a>тип ресурса tenantTag

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тег, который может быть назначен управляемому клиенту.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список tenantTags](../api/managedtenants-managedtenant-list-tenanttags.md)|[коллекция microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Получите список объектов [tenantTag](../resources/managedtenants-tenanttag.md) и их свойств.|
|[Создание tenantTag](../api/managedtenants-managedtenant-post-tenanttags.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Создание нового [объекта tenantTag.](../resources/managedtenants-tenanttag.md)|
|[Get tenantTag](../api/managedtenants-tenanttag-get.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Ознакомьтесь с свойствами и отношениями объекта [tenantTag.](../resources/managedtenants-tenanttag.md)|
|[Обновление tenantTag](../api/managedtenants-tenanttag-update.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Обновление свойств объекта [tenantTag.](../resources/managedtenants-tenanttag.md)|
|[Удаление tenantTag](../api/managedtenants-tenanttag-delete.md)|Нет|Удаляет объект [tenantTag.](../resources/managedtenants-tenanttag.md)|
|[assignTag](../api/managedtenants-tenanttag-assigntag.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Назначает тег клиента указанным управляемым арендаторам.|
|[unassignTag](../api/managedtenants-tenanttag-unassigntag.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Un-assigns the tenant tag from the specified managed tenants.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdByUserId|String|Идентификатор учетной записи, создав тег клиента. Обязательный. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания тега клиента. Обязательный. Только для чтения.|
|deletedDateTime|DateTimeOffset|Дата и время удаления тега клиента. Обязательный. Только для чтения.|
|description|String|Описание тега клиента. Необязательно. Только для чтения.|
|displayName|String|Имя отображения тега клиента. Обязательный. Только для чтения.|
|id|String|Уникальный идентификатор тега клиента. Обязательный. Только для чтения.|
|lastActionByUserId|String|Идентификатор учетной записи, которая продолжалась на теге клиента. Необязательно. Только для чтения.|
|lastActionDateTime|DateTimeOffset|Дата и время выполнения последнего действия по тегу клиента. Необязательно. Только для чтения.|
|клиенты|[коллекция microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md)|Коллекция управляемых клиентов, связанных с тегом клиента. Необязательное.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantTag",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdByUserId": "String",
  "lastActionByUserId": "String",
  "tenants": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
    }
  ],
  "lastActionDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)"
}
```
