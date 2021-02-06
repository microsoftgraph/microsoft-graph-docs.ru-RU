---
title: Тип ресурса accessPackageLocalizedContent
description: Сложный тип, используемый для представления текста на разных локальных уровнях вместе с текстом по умолчанию.*
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 155d0ffd8f7f705c79bd753aa26f659968b87829
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137356"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a>Тип ресурса accessPackageLocalizedContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, используемый для представления текста в нескольких локализованных формах. Он включает текст по умолчанию, который используется в любом случае, когда запрашиваемая локализация недоступна.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultText|Строка|Строка отката, которая используется, когда запрашиваемая локализация недоступна. Обязательный элемент. |
|localizedTexts|[Коллекция accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md)|Контент, представленный в формате для определенного локали. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedContent",
  "defaultText": "String",
  "localizedTexts": [
    {
      "@odata.type": "microsoft.graph.accessPackageLocalizedText"
    }
  ]
}
```
