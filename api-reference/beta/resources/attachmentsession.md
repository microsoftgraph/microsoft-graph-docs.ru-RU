---
title: Тип ресурса attachmentSession
description: Представляет ресурс, который отправляет большие вложения в todoTask.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 71be9f9afb61735341f98e77b7790b724fcd036a
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645715"
---
# <a name="attachmentsession-resource-type"></a>Тип ресурса attachmentSession

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс, который отправляет большие вложения в [todoTask](../resources/todotask.md).

Наследует [от сущности](../resources/entity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|содержимое|Поток|Отправляемые потоки содержимого.|
|expirationDateTime|DateTimeOffset| Дата и время окончания срока действия сеанса отправки в формате UTC. Полный файл необходимо отправить до наступления этого момента.|
|id|String|Уникальный идентификатор сеанса вложения. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|nextExpectedRanges|Коллекция строк|Указывает одно значение, представляющее `{start}` расположение в файле, где должна начаться следующая отправка.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachmentSession",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentSession",
  "content": "Stream",
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "nextExpectedRanges": [
    "String"
  ]
}
```

