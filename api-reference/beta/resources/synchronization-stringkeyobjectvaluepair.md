---
title: Тип ресурса Стрингкэйобжектвалуепаир
description: Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523219"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="453ae-104">Тип ресурса Стрингкэйобжектвалуепаир</span><span class="sxs-lookup"><span data-stu-id="453ae-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="453ae-105">Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="453ae-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="453ae-106">Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="453ae-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="453ae-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="453ae-107">Properties</span></span>
| <span data-ttu-id="453ae-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="453ae-108">Property</span></span>     | <span data-ttu-id="453ae-109">Тип</span><span class="sxs-lookup"><span data-stu-id="453ae-109">Type</span></span>   |<span data-ttu-id="453ae-110">Описание</span><span class="sxs-lookup"><span data-stu-id="453ae-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="453ae-111">ключа</span><span class="sxs-lookup"><span data-stu-id="453ae-111">key</span></span>|<span data-ttu-id="453ae-112">String</span><span class="sxs-lookup"><span data-stu-id="453ae-112">String</span></span>|<span data-ttu-id="453ae-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="453ae-113">Key.</span></span>|
|<span data-ttu-id="453ae-114">значение</span><span class="sxs-lookup"><span data-stu-id="453ae-114">value</span></span>|<span data-ttu-id="453ae-115">Любые</span><span class="sxs-lookup"><span data-stu-id="453ae-115">Any</span></span>|<span data-ttu-id="453ae-116">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="453ae-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="453ae-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="453ae-117">JSON representation</span></span>

<span data-ttu-id="453ae-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="453ae-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyobjectvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
