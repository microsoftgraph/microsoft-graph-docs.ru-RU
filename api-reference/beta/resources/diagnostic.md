---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждении для операции OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f0d5e6a938c454ca2efeda0dd7628c15269d6311
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507242"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="34cba-103">Тип ресурса диагностики</span><span class="sxs-lookup"><span data-stu-id="34cba-103">diagnostic resource type</span></span>

<span data-ttu-id="34cba-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="34cba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34cba-105">Сведения об ошибке или предупреждении для операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="34cba-105">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34cba-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34cba-106">JSON representation</span></span>

<span data-ttu-id="34cba-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="34cba-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="34cba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="34cba-108">Properties</span></span>
| <span data-ttu-id="34cba-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="34cba-109">Property</span></span>     | <span data-ttu-id="34cba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="34cba-110">Type</span></span>   |<span data-ttu-id="34cba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="34cba-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34cba-112">message</span><span class="sxs-lookup"><span data-stu-id="34cba-112">message</span></span>|<span data-ttu-id="34cba-113">String</span><span class="sxs-lookup"><span data-stu-id="34cba-113">String</span></span>|<span data-ttu-id="34cba-114">Сообщение с описанием условия, вызвавшего ошибку или предупреждение.</span><span class="sxs-lookup"><span data-stu-id="34cba-114">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="34cba-115">url</span><span class="sxs-lookup"><span data-stu-id="34cba-115">url</span></span>|<span data-ttu-id="34cba-116">String</span><span class="sxs-lookup"><span data-stu-id="34cba-116">String</span></span>|<span data-ttu-id="34cba-117">Ссылка на документацию по этой ошибке.</span><span class="sxs-lookup"><span data-stu-id="34cba-117">The link to the documentation for this issue.</span></span>|

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
