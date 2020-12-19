---
title: Тип ресурса accessPackageAnswerChoice
description: Параметр ответа для accessPackageMultipleChoiceQuestion.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f34656a72d217adec1ff46be689b283461332fb
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720419"
---
# <a name="accesspackageanswerchoice-resource-type"></a>Тип ресурса accessPackageAnswerChoice

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает параметр ответа для [accessPackageMultipleChoiceQuestion.](../resources/accesspackagemultiplechoicequestion.md) Несколько accessPackageAnswerChoices можно добавить в [accessPackageMultipleChoiceQuestion.](../resources/accesspackagemultiplechoicequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actualValue|String|Фактическое значение выбранного выбора. Как правило, это строковое значение, понятное приложениям. Обязательный. |
|displayValue|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Локализованные отображаемые значения, которые отображаются для запрашивающих и утвержденных. Обязательный.

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerChoice",
  "actualValue": "String",
  "displayValue": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  }
}
```
