---
title: Тип ресурса УнмутепартиЦипантоператион
description: Описывает формат ответа для функции "без звука".
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9ebb8d749f8cbe6ce01711ca6a0c36b134e8369
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519598"
---
# <a name="unmuteparticipantoperation-resource-type"></a><span data-ttu-id="dfa8c-103">Тип ресурса УнмутепартиЦипантоператион</span><span class="sxs-lookup"><span data-stu-id="dfa8c-103">unmuteParticipantOperation resource type</span></span>

<span data-ttu-id="dfa8c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dfa8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfa8c-105">Описывает формат ответа для функции "без звука".</span><span class="sxs-lookup"><span data-stu-id="dfa8c-105">Describes the response format of a call participant unmute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="dfa8c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfa8c-106">Properties</span></span>

| <span data-ttu-id="dfa8c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfa8c-107">Property</span></span>                       | <span data-ttu-id="dfa8c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dfa8c-108">Type</span></span>                        | <span data-ttu-id="dfa8c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa8c-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="dfa8c-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="dfa8c-110">clientContext</span></span>                  | <span data-ttu-id="dfa8c-111">String</span><span class="sxs-lookup"><span data-stu-id="dfa8c-111">String</span></span>                      | <span data-ttu-id="dfa8c-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-112">Unique client context string.</span></span> <span data-ttu-id="dfa8c-113">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="dfa8c-114">id</span><span class="sxs-lookup"><span data-stu-id="dfa8c-114">id</span></span>                             | <span data-ttu-id="dfa8c-115">Строка</span><span class="sxs-lookup"><span data-stu-id="dfa8c-115">String</span></span>                      | <span data-ttu-id="dfa8c-116">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-116">The server operation ID.</span></span> <span data-ttu-id="dfa8c-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="dfa8c-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="dfa8c-118">resultInfo</span></span>                     | [<span data-ttu-id="dfa8c-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="dfa8c-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="dfa8c-120">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-120">The result information.</span></span>  <span data-ttu-id="dfa8c-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="dfa8c-122">status</span><span class="sxs-lookup"><span data-stu-id="dfa8c-122">status</span></span>                         | <span data-ttu-id="dfa8c-123">String</span><span class="sxs-lookup"><span data-stu-id="dfa8c-123">String</span></span>                      | <span data-ttu-id="dfa8c-124">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="dfa8c-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="dfa8c-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="dfa8c-126">Relationships</span></span>
<span data-ttu-id="dfa8c-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfa8c-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dfa8c-128">JSON representation</span></span>

<span data-ttu-id="dfa8c-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfa8c-129">The following is a JSON representation of the resource.</span></span>

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
