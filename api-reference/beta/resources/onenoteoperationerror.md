---
title: Тип ресурса Оненотеоператионеррор
description: Ошибка при выполнении операции с OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8b2912ee02ab22631224b892a09a8c4dd7840dd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341449"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="0b740-103">Тип ресурса Оненотеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="0b740-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b740-104">Ошибка при выполнении операции с OneNote.</span><span class="sxs-lookup"><span data-stu-id="0b740-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b740-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b740-105">JSON representation</span></span>

<span data-ttu-id="0b740-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b740-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0b740-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b740-107">Properties</span></span>
| <span data-ttu-id="0b740-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b740-108">Property</span></span>     | <span data-ttu-id="0b740-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0b740-109">Type</span></span>   |<span data-ttu-id="0b740-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0b740-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b740-111">code</span><span class="sxs-lookup"><span data-stu-id="0b740-111">code</span></span>|<span data-ttu-id="0b740-112">string</span><span class="sxs-lookup"><span data-stu-id="0b740-112">string</span></span>|<span data-ttu-id="0b740-113">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="0b740-113">The error code.</span></span>|
|<span data-ttu-id="0b740-114">message</span><span class="sxs-lookup"><span data-stu-id="0b740-114">message</span></span>|<span data-ttu-id="0b740-115">string</span><span class="sxs-lookup"><span data-stu-id="0b740-115">string</span></span>|<span data-ttu-id="0b740-116">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0b740-116">The error message.</span></span>|

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
