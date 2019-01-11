---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждение для выполнения операции OneNote.
localization_priority: Normal
ms.openlocfilehash: 28cdd1c07bab0494a69cfb7ce6a5284238e1ff19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845992"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="da565-103">Тип ресурса диагностики</span><span class="sxs-lookup"><span data-stu-id="da565-103">diagnostic resource type</span></span>

> <span data-ttu-id="da565-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da565-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da565-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da565-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da565-106">Сведения об ошибке или предупреждение для выполнения операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="da565-106">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da565-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da565-107">JSON representation</span></span>

<span data-ttu-id="da565-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="da565-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="da565-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="da565-109">Properties</span></span>
| <span data-ttu-id="da565-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="da565-110">Property</span></span>     | <span data-ttu-id="da565-111">Тип</span><span class="sxs-lookup"><span data-stu-id="da565-111">Type</span></span>   |<span data-ttu-id="da565-112">Описание</span><span class="sxs-lookup"><span data-stu-id="da565-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da565-113">message</span><span class="sxs-lookup"><span data-stu-id="da565-113">message</span></span>|<span data-ttu-id="da565-114">String</span><span class="sxs-lookup"><span data-stu-id="da565-114">String</span></span>|<span data-ttu-id="da565-115">Сообщение, описывающее условие, инициирующую сообщение об ошибке или предупреждение.</span><span class="sxs-lookup"><span data-stu-id="da565-115">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="da565-116">url</span><span class="sxs-lookup"><span data-stu-id="da565-116">url</span></span>|<span data-ttu-id="da565-117">String</span><span class="sxs-lookup"><span data-stu-id="da565-117">String</span></span>|<span data-ttu-id="da565-118">Ссылка на документацию для этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="da565-118">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
