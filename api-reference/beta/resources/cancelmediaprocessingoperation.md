---
title: Тип ресурса Канцелмедиапроцессингоператион
description: Этот тип ресурса используется для описания формата ответа операции отмены обработки мультимедиа.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc9142be9524b34ded7a2bd9315a6bb2cc1aa9ca
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006728"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="2ad5a-103">Тип ресурса Канцелмедиапроцессингоператион</span><span class="sxs-lookup"><span data-stu-id="2ad5a-103">CancelMediaProcessingOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ad5a-104">Описывает формат ответа для операции отмены обработки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-104">Describes the response format of media processing cancel operation.</span></span>

## <a name="properties"></a><span data-ttu-id="2ad5a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ad5a-105">Properties</span></span>

| <span data-ttu-id="2ad5a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ad5a-106">Property</span></span>                       | <span data-ttu-id="2ad5a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2ad5a-107">Type</span></span>                        | <span data-ttu-id="2ad5a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2ad5a-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2ad5a-109">ко</span><span class="sxs-lookup"><span data-stu-id="2ad5a-109">all</span></span>                            | <span data-ttu-id="2ad5a-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad5a-110">Boolean</span></span>                     | <span data-ttu-id="2ad5a-111">Указывает, следует ли остановить все операции или текущие.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-111">Indicates whether to stop all operations or current.</span></span>                                                                                    |
| <span data-ttu-id="2ad5a-112">Контекст</span><span class="sxs-lookup"><span data-stu-id="2ad5a-112">clientContext</span></span>                  | <span data-ttu-id="2ad5a-113">String</span><span class="sxs-lookup"><span data-stu-id="2ad5a-113">String</span></span>                      | <span data-ttu-id="2ad5a-114">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-114">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="2ad5a-115">id</span><span class="sxs-lookup"><span data-stu-id="2ad5a-115">id</span></span>                             | <span data-ttu-id="2ad5a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="2ad5a-116">String</span></span>                      | <span data-ttu-id="2ad5a-117">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-117">The server operation ID.</span></span> <span data-ttu-id="2ad5a-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-118">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="2ad5a-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2ad5a-119">resultInfo</span></span>                     | [<span data-ttu-id="2ad5a-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2ad5a-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="2ad5a-121">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-121">The result information.</span></span>  <span data-ttu-id="2ad5a-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-122">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="2ad5a-123">status</span><span class="sxs-lookup"><span data-stu-id="2ad5a-123">status</span></span>                         | <span data-ttu-id="2ad5a-124">String</span><span class="sxs-lookup"><span data-stu-id="2ad5a-124">String</span></span>                      | <span data-ttu-id="2ad5a-125">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="2ad5a-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-126">Read-only.</span></span>                                                  |

## <a name="relationships"></a><span data-ttu-id="2ad5a-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="2ad5a-127">Relationships</span></span>
<span data-ttu-id="2ad5a-128">Нет</span><span class="sxs-lookup"><span data-stu-id="2ad5a-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ad5a-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ad5a-129">JSON representation</span></span>

<span data-ttu-id="2ad5a-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ad5a-130">The following is a JSON representation of the resource.</span></span>

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
