---
title: Тип ресурса Канцелмедиапроцессингоператион
description: Этот тип ресурса используется для описания формата ответа операции отмены обработки мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20da55c068f6e0f0a69b876cfd23181eac1391a4
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913501"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="67439-103">Тип ресурса Канцелмедиапроцессингоператион</span><span class="sxs-lookup"><span data-stu-id="67439-103">CancelMediaProcessingOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67439-104">Описывает формат ответа для операции отмены обработки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="67439-104">Describes the response format of media processing cancel operation.</span></span>

## <a name="properties"></a><span data-ttu-id="67439-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="67439-105">Properties</span></span>

| <span data-ttu-id="67439-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="67439-106">Property</span></span>                       | <span data-ttu-id="67439-107">Тип</span><span class="sxs-lookup"><span data-stu-id="67439-107">Type</span></span>                        | <span data-ttu-id="67439-108">Описание</span><span class="sxs-lookup"><span data-stu-id="67439-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="67439-109">ко</span><span class="sxs-lookup"><span data-stu-id="67439-109">all</span></span>                            | <span data-ttu-id="67439-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="67439-110">Boolean</span></span>                     | <span data-ttu-id="67439-111">Указывает, следует ли остановить все операции или текущие.</span><span class="sxs-lookup"><span data-stu-id="67439-111">Indicates whether to stop all operations or current.</span></span>                                                                                    |
| <span data-ttu-id="67439-112">Контекст</span><span class="sxs-lookup"><span data-stu-id="67439-112">clientContext</span></span>                  | <span data-ttu-id="67439-113">String</span><span class="sxs-lookup"><span data-stu-id="67439-113">String</span></span>                      | <span data-ttu-id="67439-114">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="67439-114">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="67439-115">id</span><span class="sxs-lookup"><span data-stu-id="67439-115">id</span></span>                             | <span data-ttu-id="67439-116">Строка</span><span class="sxs-lookup"><span data-stu-id="67439-116">String</span></span>                      | <span data-ttu-id="67439-117">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="67439-117">The server operation ID.</span></span> <span data-ttu-id="67439-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67439-118">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="67439-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="67439-119">resultInfo</span></span>                     | [<span data-ttu-id="67439-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="67439-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="67439-121">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="67439-121">The result information.</span></span>  <span data-ttu-id="67439-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67439-122">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="67439-123">status</span><span class="sxs-lookup"><span data-stu-id="67439-123">status</span></span>                         | <span data-ttu-id="67439-124">String</span><span class="sxs-lookup"><span data-stu-id="67439-124">String</span></span>                      | <span data-ttu-id="67439-125">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="67439-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="67439-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67439-126">Read-only.</span></span>                                                  |

## <a name="relationships"></a><span data-ttu-id="67439-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="67439-127">Relationships</span></span>
<span data-ttu-id="67439-128">Нет</span><span class="sxs-lookup"><span data-stu-id="67439-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67439-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67439-129">JSON representation</span></span>

<span data-ttu-id="67439-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67439-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
}-->
```json
{
  "all": true,
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
  "description": "cancelMediaProcessingOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
