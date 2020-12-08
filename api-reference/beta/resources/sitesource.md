---
title: Тип ресурса Ситесаурце
description: Контейнер для сайта, связанного с хранитель.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 60b2d8fb3374dd4f97dcff802caf509e66ca6db1
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597825"
---
# <a name="sitesource-resource-type"></a>Тип ресурса Ситесаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для сайта, связанного с [хранитель](custodian.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Ситесаурцес](../api/custodian-list-sitesources.md)|Коллекция [ситесаурце](../resources/sitesource.md)|Получение списка объектов **ситесаурце** и их свойств.|
|[Создание Ситесаурце](../api/custodian-post-sitesources.md)|[ситесаурце](../resources/sitesource.md)|Создание нового объекта **ситесаурце** .|
|[Получение Ситесаурце](../api/sitesource-get.md)|[ситесаурце](../resources/sitesource.md)|Чтение свойств и связей объекта **ситесаурце** .|
|[Удаление Ситесаурце](../api/sitesource-delete.md)|Нет|Удаление объекта **ситесаурце** .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **ситесаурце**.|
|createdDateTime|DateTimeOffset|Дата и время создания **ситесаурце** .|
|displayName|String|Отображаемое имя **ситесаурце**. Это будет имя сайта SharePoint.|
|id|String| Идентификатор **ситесаурце**. Это значение не является ИДЕНТИФИКАТОРом действительного сайта.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|site|[site](../resources/site.md)|Сайт SharePoint, связанный с **ситесаурце**.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.siteSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
