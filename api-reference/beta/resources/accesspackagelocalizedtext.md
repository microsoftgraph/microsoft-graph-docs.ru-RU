---
title: Тип ресурса accessPackageLocalizedText
description: Сложный тип, используемый для представления строки на определенном языке.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8d493f0909617dcda26546ccc262d7591c6b9309
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137349"
---
# <a name="accesspackagelocalizedtext-resource-type"></a>Тип ресурса accessPackageLocalizedText

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, используемый для представления строки на определенном языке.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|languageCode|Строка|Код ISO для намечаемого языка. Обязательный элемент. |
|текст|Строка|Текст на определенном языке. Обязательный. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedText",
  "text": "String",
  "languageCode": "String"
}
```
