---
title: Тип ресурса Довнградежустификатион
description: Представляет ввод пользователя по причине выполнения возврата к предыдущей версии.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aacc32ac86df4eda087f49dbb3dca05a356e8080
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939427"
---
# <a name="downgradejustification-resource-type"></a><span data-ttu-id="0a709-103">Тип ресурса Довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="0a709-103">downgradeJustification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a709-104">Представляет ввод пользователя по причине выполнения возврата к предыдущей версии.</span><span class="sxs-lookup"><span data-stu-id="0a709-104">Represents user input on why downgrade was performed.</span></span> <span data-ttu-id="0a709-105">Выравнивание на более ранней версии может потребоваться на основе конфигурации политики меток в центре безопасности и соответствия требованиям Office.</span><span class="sxs-lookup"><span data-stu-id="0a709-105">Downgrade justification might be required based on label policy configuration in Office Security and Compliance Center.</span></span>

## <a name="properties"></a><span data-ttu-id="0a709-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a709-106">Properties</span></span>

| <span data-ttu-id="0a709-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a709-107">Property</span></span>             | <span data-ttu-id="0a709-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0a709-108">Type</span></span>    | <span data-ttu-id="0a709-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0a709-109">Description</span></span>                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0a709-110">исдовнградежустифиед</span><span class="sxs-lookup"><span data-stu-id="0a709-110">isDowngradeJustified</span></span> | <span data-ttu-id="0a709-111">Логический</span><span class="sxs-lookup"><span data-stu-id="0a709-111">Boolean</span></span> | <span data-ttu-id="0a709-112">Указывает, является ли переход на предыдущее или не выровненный.</span><span class="sxs-lookup"><span data-stu-id="0a709-112">Indicates whether the downgrade is or is not justified.</span></span>                                              |
| <span data-ttu-id="0a709-113">жустификатионмессаже</span><span class="sxs-lookup"><span data-stu-id="0a709-113">justificationMessage</span></span> | <span data-ttu-id="0a709-114">Строка</span><span class="sxs-lookup"><span data-stu-id="0a709-114">String</span></span>  | <span data-ttu-id="0a709-115">Сообщение, указывающее, почему выравниваются более ранние версии.</span><span class="sxs-lookup"><span data-stu-id="0a709-115">Message that indicates why a downgrade is justified.</span></span> <span data-ttu-id="0a709-116">Сообщение будет отображаться в разделе Журналы администрирования.</span><span class="sxs-lookup"><span data-stu-id="0a709-116">The message will appear in administrative logs.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a709-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a709-117">JSON representation</span></span>

<span data-ttu-id="0a709-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a709-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.downgradeJustification",
  "baseType": null
}-->

```json
{
  "isDowngradeJustified": true,
  "justificationMessage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "downgradeJustification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->