---
title: Тип ресурса accessPackageLocalizedContent
description: Сложный тип, используемый для представления текста на разных локальных уровнях вместе с текстом по умолчанию.*
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91ef87428b4171317943e9ecf1ec92e959c7a62b
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720328"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a>Тип ресурса accessPackageLocalizedContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, используемый для представления текста в нескольких локализованных формах. Он включает текст по умолчанию, который используется в любом случае, когда запрашиваемая локализация недоступна.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultText|String|Строка отката, которая используется, когда запрашиваемая локализация недоступна. Обязательный. |
|localizedTexts|[Коллекция accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md)|Контент, представленный в формате для определенного локали. |

## <a name="relationships"></a>Отношения
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
