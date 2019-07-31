---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждении для операции OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4ac591640e647a1caa5230bd8e7e8c64ad2314af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973153"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="fcf25-103">Тип ресурса диагностики</span><span class="sxs-lookup"><span data-stu-id="fcf25-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcf25-104">Сведения об ошибке или предупреждении для операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="fcf25-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcf25-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcf25-105">JSON representation</span></span>

<span data-ttu-id="fcf25-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="fcf25-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="fcf25-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcf25-107">Properties</span></span>
| <span data-ttu-id="fcf25-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcf25-108">Property</span></span>     | <span data-ttu-id="fcf25-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fcf25-109">Type</span></span>   |<span data-ttu-id="fcf25-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf25-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcf25-111">message</span><span class="sxs-lookup"><span data-stu-id="fcf25-111">message</span></span>|<span data-ttu-id="fcf25-112">String</span><span class="sxs-lookup"><span data-stu-id="fcf25-112">String</span></span>|<span data-ttu-id="fcf25-113">Сообщение с описанием условия, вызвавшего ошибку или предупреждение.</span><span class="sxs-lookup"><span data-stu-id="fcf25-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="fcf25-114">url</span><span class="sxs-lookup"><span data-stu-id="fcf25-114">url</span></span>|<span data-ttu-id="fcf25-115">String</span><span class="sxs-lookup"><span data-stu-id="fcf25-115">String</span></span>|<span data-ttu-id="fcf25-116">Ссылка на документацию по этой ошибке.</span><span class="sxs-lookup"><span data-stu-id="fcf25-116">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
