---
title: Тип ресурса dataSource
description: Объект DataSource — абстрактный базовый класс
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 645ae33eb6c43972122623e52bfecf17f39491e4
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597830"
---
# <a name="datasource-resource-type"></a>Тип ресурса dataSource

Пространство имен: microsoft.graph

Сущность dataSource — это абстрактный объект BaseClass, используемый для определения источников контента для обнаружения электронных данных.

## <a name="methods"></a>Methods

Нет

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **источник данных**.|
|createdDateTime|DateTimeOffset|Дата и время создания **источника данных** .|
|displayName|String|Отображаемое имя **источника данных**. Это будет имя сайта SharePoint.|
|id|String| Идентификатор **источника данных**. Это значение не является ИДЕНТИФИКАТОРом действительного сайта.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
