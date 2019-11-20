---
title: Тип ресурса УнмутепартиЦипантоператион
description: Описывает формат ответа для функции "без звука".
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d3c843ffcf46d8816f4ad3853d42cb5d0fa34422
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748050"
---
# <a name="unmuteparticipantoperation-resource-type"></a><span data-ttu-id="d05a8-103">Тип ресурса УнмутепартиЦипантоператион</span><span class="sxs-lookup"><span data-stu-id="d05a8-103">unmuteParticipantOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d05a8-104">Описывает формат ответа для функции "без звука".</span><span class="sxs-lookup"><span data-stu-id="d05a8-104">Describes the response format of a call participant unmute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="d05a8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d05a8-105">Properties</span></span>

| <span data-ttu-id="d05a8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d05a8-106">Property</span></span>                       | <span data-ttu-id="d05a8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d05a8-107">Type</span></span>                        | <span data-ttu-id="d05a8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d05a8-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d05a8-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="d05a8-109">clientContext</span></span>                  | <span data-ttu-id="d05a8-110">Строка</span><span class="sxs-lookup"><span data-stu-id="d05a8-110">String</span></span>                      | <span data-ttu-id="d05a8-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="d05a8-111">Unique client context string.</span></span> <span data-ttu-id="d05a8-112">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="d05a8-112">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="d05a8-113">id</span><span class="sxs-lookup"><span data-stu-id="d05a8-113">id</span></span>                             | <span data-ttu-id="d05a8-114">Строка</span><span class="sxs-lookup"><span data-stu-id="d05a8-114">String</span></span>                      | <span data-ttu-id="d05a8-115">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="d05a8-115">The server operation ID.</span></span> <span data-ttu-id="d05a8-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d05a8-116">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="d05a8-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d05a8-117">resultInfo</span></span>                     | [<span data-ttu-id="d05a8-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d05a8-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d05a8-119">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="d05a8-119">The result information.</span></span>  <span data-ttu-id="d05a8-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d05a8-120">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="d05a8-121">status</span><span class="sxs-lookup"><span data-stu-id="d05a8-121">status</span></span>                         | <span data-ttu-id="d05a8-122">String</span><span class="sxs-lookup"><span data-stu-id="d05a8-122">String</span></span>                      | <span data-ttu-id="d05a8-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d05a8-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d05a8-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d05a8-124">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="d05a8-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="d05a8-125">Relationships</span></span>
<span data-ttu-id="d05a8-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d05a8-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d05a8-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d05a8-127">JSON representation</span></span>

<span data-ttu-id="d05a8-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d05a8-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unmuteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
