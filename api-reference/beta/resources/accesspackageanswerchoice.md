---
title: Тип ресурса accessPackageAnswerChoice
description: Параметр ответа для accessPackageMultipleChoiceQuestion.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c7fc7db1c9360146c2f62fd9048ad0db3d58b80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135480"
---
# <a name="accesspackageanswerchoice-resource-type"></a>Тип ресурса accessPackageAnswerChoice

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает параметр ответа для [accessPackageMultipleChoiceQuestion.](../resources/accesspackagemultiplechoicequestion.md) В accessPackageMultipleChoices можно добавить несколько [accessPackageAnswerChoiceQuestion.](../resources/accesspackagemultiplechoicequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actualValue|Строка|Фактическое значение выбранного выбора. Как правило, это строковое значение, понятное приложениям. Обязательный элемент. |
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
