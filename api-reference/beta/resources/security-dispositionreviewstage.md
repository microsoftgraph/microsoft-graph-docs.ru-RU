---
title: Тип ресурса dispositionReviewStage
description: Представляет многоуровневый процесс проверки, в котором рецензенты указывают на каждом этапе ликвидации, следует ли удалять или сохранять элемент контента.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: cc89d8c907fcd6ec84c4810f30e19921e6312d1c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447815"
---
# <a name="dispositionreviewstage-resource-type"></a>Тип ресурса dispositionReviewStage

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет многоуровневый процесс проверки, в котором рецензенты указывают на каждом этапе ликвидации, следует ли удалять или сохранять элемент контента.
Дополнительные сведения см. [в разделе "Ликвидация содержимого"](/microsoft-365/compliance/disposition).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание retentionLabel](../api/security-retentionlabel-post.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Создайте объект [retentionLabel](../resources/security-retentionlabel.md) . |
|[Обновление retentionLabel](../api/security-retentionlabel-update.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Обновите [объект retentionLabel](../resources/security-retentionlabel.md) . |


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для каждого этапа. |
|name|String|Имя, представляющее каждый этап в коллекции. |
|reviewersEmailAddresses|Коллекция String|Коллекция рецензентов на каждом этапе. |
|stageNumber|Int32|Порядковый номер для каждого этапа проверки перед ликвидацией. |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dispositionReviewStage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dispositionReviewStage",
  "id": "String (identifier)",
  "stageNumber": "Integer",
  "name": "String",
  "reviewersEmailAddresses": [
    "String"
  ]
}
```
