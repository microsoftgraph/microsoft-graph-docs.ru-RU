---
title: Тип ресурса Оненотеоператионеррор
description: Ошибка при выполнении операции с OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ecd1c42ceb278c483601344dd28c72f7436b9537
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009351"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="7f78d-103">Тип ресурса Оненотеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="7f78d-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f78d-104">Ошибка при выполнении операции с OneNote.</span><span class="sxs-lookup"><span data-stu-id="7f78d-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f78d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f78d-105">JSON representation</span></span>

<span data-ttu-id="7f78d-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f78d-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="7f78d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f78d-107">Properties</span></span>
| <span data-ttu-id="7f78d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f78d-108">Property</span></span>     | <span data-ttu-id="7f78d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7f78d-109">Type</span></span>   |<span data-ttu-id="7f78d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f78d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f78d-111">code</span><span class="sxs-lookup"><span data-stu-id="7f78d-111">code</span></span>|<span data-ttu-id="7f78d-112">string</span><span class="sxs-lookup"><span data-stu-id="7f78d-112">string</span></span>|<span data-ttu-id="7f78d-113">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="7f78d-113">The error code.</span></span>|
|<span data-ttu-id="7f78d-114">message</span><span class="sxs-lookup"><span data-stu-id="7f78d-114">message</span></span>|<span data-ttu-id="7f78d-115">string</span><span class="sxs-lookup"><span data-stu-id="7f78d-115">string</span></span>|<span data-ttu-id="7f78d-116">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7f78d-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
