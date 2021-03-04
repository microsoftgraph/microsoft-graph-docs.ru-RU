---
title: тип ресурсов unifiedGroupSource
description: Контейнер для группы хранителя.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b6d1b1d1a7d3abee2516e170fcead20c73235f1f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447543"
---
# <a name="unifiedgroupsource-resource-type"></a>тип ресурсов unifiedGroupSource

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для [группы](ediscovery-custodian.md) хранителя.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список унифицированныхGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)|[коллекция microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Получите список объектов **unifiedGroupSource** и их свойств.|
|[Создание unifiedGroupSource](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Создание нового **объекта unifiedGroupSource.**|
|[Get unifiedGroupSource](../api/ediscovery-unifiedgroupsource-get.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Ознакомьтесь с свойствами и отношениями объекта **unifiedGroupSource.**|
|[Удаление unifiedGroupSource](../api/ediscovery-unifiedgroupsource-delete.md)|Нет|Удаление **объекта unifiedGroupSource.**|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **унифицированнуюGroupSource.**|
|createdDateTime|DateTimeOffset|Дата и время создания **unifiedGroupSource.**|
|displayName|String|Отображаемое имя единой группы — это имя группы.|
|id|String|ID **единойGroupSource**. Это не ID фактической группы.|
|includedSources|microsoft.graph.ediscovery.sourceType|Указывает, какие источники включены в эту группу. Возможные значения: `mailbox`, `site`.|

### <a name="sourcetype-values"></a>значения sourceType

Типы источников, связанных с пользователем. Включает почтовый ящик и сайт по умолчанию.

|Member|Описание|
|:----|-----------|
|mailbox|Представляет почтовый ящик.|
|site|Представляет сайт SharePoint.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|group|[group](../resources/group.md)|Группа, связанная с **унифицированнойGroupSource**.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
