---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждение для выполнения операции OneNote.
ms.openlocfilehash: 29e30d44a9fde91b79778042be19461b880216ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080618"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="2bb94-103">Тип ресурса диагностики</span><span class="sxs-lookup"><span data-stu-id="2bb94-103">diagnostic resource type</span></span>

> <span data-ttu-id="2bb94-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2bb94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bb94-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bb94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bb94-106">Сведения об ошибке или предупреждение для выполнения операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="2bb94-106">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bb94-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2bb94-107">JSON representation</span></span>

<span data-ttu-id="2bb94-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="2bb94-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2bb94-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2bb94-109">Properties</span></span>
| <span data-ttu-id="2bb94-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bb94-110">Property</span></span>     | <span data-ttu-id="2bb94-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2bb94-111">Type</span></span>   |<span data-ttu-id="2bb94-112">Description</span><span class="sxs-lookup"><span data-stu-id="2bb94-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bb94-113">message</span><span class="sxs-lookup"><span data-stu-id="2bb94-113">message</span></span>|<span data-ttu-id="2bb94-114">String</span><span class="sxs-lookup"><span data-stu-id="2bb94-114">String</span></span>|<span data-ttu-id="2bb94-115">Сообщение, описывающее условие, инициирующую сообщение об ошибке или предупреждение.</span><span class="sxs-lookup"><span data-stu-id="2bb94-115">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="2bb94-116">url</span><span class="sxs-lookup"><span data-stu-id="2bb94-116">url</span></span>|<span data-ttu-id="2bb94-117">String</span><span class="sxs-lookup"><span data-stu-id="2bb94-117">String</span></span>|<span data-ttu-id="2bb94-118">Ссылка на документацию для этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="2bb94-118">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->