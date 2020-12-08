---
title: Тип ресурса Унифиедграупсаурце
description: Контейнер для группы хранитель.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 5fba2a994cda61f111739d98ea3a210c76ffeb23
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597813"
---
# <a name="unifiedgroupsource-resource-type"></a>Тип ресурса Унифиедграупсаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для группы [хранитель](custodian.md) .

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Унифиедграупсаурцес](../api/custodian-list-unifiedgroupsources.md)|Коллекция [унифиедграупсаурце](../resources/unifiedgroupsource.md)|Получение списка объектов **унифиедграупсаурце** и их свойств.|
|[Создание Унифиедграупсаурце](../api/custodian-post-unifiedgroupsources.md)|[унифиедграупсаурце](../resources/unifiedgroupsource.md)|Создание нового объекта **унифиедграупсаурце** .|
|[Получение Унифиедграупсаурце](../api/unifiedgroupsource-get.md)|[унифиедграупсаурце](../resources/unifiedgroupsource.md)|Чтение свойств и связей объекта **унифиедграупсаурце** .|
|[Удаление Унифиедграупсаурце](../api/unifiedgroupsource-delete.md)|Нет|Удаление объекта **унифиедграупсаурце** .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **унифиедграупсаурце**.|
|createdDateTime|DateTimeOffset|Дата и время создания **унифиедграупсаурце** .|
|displayName|String|Отображаемое имя единой группы — это имя группы.|
|id|String|Идентификатор **унифиедграупсаурце**. Это значение не является ИДЕНТИФИКАТОРом фактической группы.|
|инклудедсаурцес|sourceType|Указывает, какие источники включены в эту группу. Возможные значения: `mailbox`, `site`.|

### <a name="sourcetype-values"></a>значения sourceType

Типы источника, связанные с пользователем. По умолчанию включается почтовый ящик и сайт.

|Member|Описание|
|:----|-----------|
|mailbox|Представляет почтовый ящик.|
|site|Представляет сайт SharePoint.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|group|[group](../resources/group.md)|Группа, связанная с **унифиедграупсаурце**.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedGroupSource",
  "baseType": "microsoft.graph.dataSource",
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
