---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждении для операции OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: b6cad8680b00b935dbaac817d53d930b5046e265
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809112"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="f9caa-103">Тип ресурса диагностики</span><span class="sxs-lookup"><span data-stu-id="f9caa-103">diagnostic resource type</span></span>

<span data-ttu-id="f9caa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9caa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9caa-105">Сведения об ошибке или предупреждении для операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="f9caa-105">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9caa-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f9caa-106">JSON representation</span></span>

<span data-ttu-id="f9caa-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f9caa-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f9caa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9caa-108">Properties</span></span>
| <span data-ttu-id="f9caa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9caa-109">Property</span></span>     | <span data-ttu-id="f9caa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9caa-110">Type</span></span>   |<span data-ttu-id="f9caa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9caa-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9caa-112">message</span><span class="sxs-lookup"><span data-stu-id="f9caa-112">message</span></span>|<span data-ttu-id="f9caa-113">String</span><span class="sxs-lookup"><span data-stu-id="f9caa-113">String</span></span>|<span data-ttu-id="f9caa-114">Сообщение с описанием условия, вызвавшего ошибку или предупреждение.</span><span class="sxs-lookup"><span data-stu-id="f9caa-114">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="f9caa-115">url</span><span class="sxs-lookup"><span data-stu-id="f9caa-115">url</span></span>|<span data-ttu-id="f9caa-116">String</span><span class="sxs-lookup"><span data-stu-id="f9caa-116">String</span></span>|<span data-ttu-id="f9caa-117">Ссылка на документацию по этой ошибке.</span><span class="sxs-lookup"><span data-stu-id="f9caa-117">The link to the documentation for this issue.</span></span>|

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
