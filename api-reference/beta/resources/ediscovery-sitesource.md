---
title: Тип ресурса siteSource
description: Контейнер для сайта, связанного с хранителями.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4fa4b8d0ccbe80ef0f65d27fa8ef648d1ea07b63
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447359"
---
# <a name="sitesource-resource-type"></a>Тип ресурса siteSource

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для сайта, связанного с [хранителями.](ediscovery-custodian.md)

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[List siteSources](../api/ediscovery-custodian-list-sitesources.md)|[коллекция microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Получите список **объектов siteSource** и их свойств.|
|[Создание siteSource](../api/ediscovery-custodian-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Создание нового **объекта siteSource.**|
|[Get siteSource](../api/ediscovery-sitesource-get.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Ознакомьтесь с свойствами и отношениями **объекта siteSource.**|
|[Удаление siteSource](../api/ediscovery-sitesource-delete.md)|Нет|Удаление **объекта siteSource.**|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **сайтSource**.|
|createdDateTime|DateTimeOffset|Дата и время **создания сайтаSource.**|
|displayName|String|Имя отображения **сайтаSource**. Это будет имя сайта SharePoint.|
|id|String| ID **сайтаSource**. Это не ID фактического сайта.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|site|[site](../resources/site.md)|Сайт SharePoint, связанный с **siteSource.**|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
