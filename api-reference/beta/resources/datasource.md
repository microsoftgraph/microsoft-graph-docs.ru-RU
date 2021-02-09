---
title: Тип ресурса dataSource
description: Объект Datasource — абстрактный базовый класс
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: c019a6b8338180584a31382c0741018791973184
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161924"
---
# <a name="datasource-resource-type"></a>Тип ресурса dataSource

Пространство имен: microsoft.graph

Объект dataSource — это абстрактный базовый класс, используемый для определения источников контента для eDiscovery.

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **dataSource.**|
|createdDateTime|DateTimeOffset|Дата и время создания **dataSource.**|
|displayName|String|Отображаемого имени **dataSource**. Это имя сайта SharePoint.|
|id|String| ИД **dataSource.** Это не ИД фактического сайта.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
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
