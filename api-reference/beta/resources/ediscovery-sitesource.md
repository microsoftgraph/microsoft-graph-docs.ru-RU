---
title: Тип ресурса siteSource
description: Контейнер для сайта, связанного с хранителями.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c178565b628728fcf6124ea3058e979f8423ce90
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080479"
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
|id|String| ID **сайтаSource**. Источник сайта можно получить в любое время с помощью [сайта Get](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|site|[site](../resources/site.md)|Сайт SharePoint, связанный **с siteSource**.|

## <a name="json-representation"></a>Представление в формате JSON

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
