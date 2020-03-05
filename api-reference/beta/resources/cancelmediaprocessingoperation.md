---
title: Тип ресурса Канцелмедиапроцессингоператион
description: Этот тип ресурса используется для описания формата ответа операции отмены обработки мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 700c63b2b620117f25df876544aeb6fb0e6d0230
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507784"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="bd272-103">Тип ресурса Канцелмедиапроцессингоператион</span><span class="sxs-lookup"><span data-stu-id="bd272-103">CancelMediaProcessingOperation resource type</span></span>

<span data-ttu-id="bd272-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bd272-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd272-105">Описывает формат ответа для операции отмены обработки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="bd272-105">Describes the response format of media processing cancel operation.</span></span>

## <a name="properties"></a><span data-ttu-id="bd272-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd272-106">Properties</span></span>

| <span data-ttu-id="bd272-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd272-107">Property</span></span>                       | <span data-ttu-id="bd272-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bd272-108">Type</span></span>                        | <span data-ttu-id="bd272-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bd272-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="bd272-110">ко</span><span class="sxs-lookup"><span data-stu-id="bd272-110">all</span></span>                            | <span data-ttu-id="bd272-111">Логический</span><span class="sxs-lookup"><span data-stu-id="bd272-111">Boolean</span></span>                     | <span data-ttu-id="bd272-112">Указывает, следует ли остановить все операции или текущие.</span><span class="sxs-lookup"><span data-stu-id="bd272-112">Indicates whether to stop all operations or current.</span></span>                                                                                    |
| <span data-ttu-id="bd272-113">Контекст</span><span class="sxs-lookup"><span data-stu-id="bd272-113">clientContext</span></span>                  | <span data-ttu-id="bd272-114">String</span><span class="sxs-lookup"><span data-stu-id="bd272-114">String</span></span>                      | <span data-ttu-id="bd272-115">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="bd272-115">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="bd272-116">id</span><span class="sxs-lookup"><span data-stu-id="bd272-116">id</span></span>                             | <span data-ttu-id="bd272-117">Строка</span><span class="sxs-lookup"><span data-stu-id="bd272-117">String</span></span>                      | <span data-ttu-id="bd272-118">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="bd272-118">The server operation ID.</span></span> <span data-ttu-id="bd272-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd272-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="bd272-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="bd272-120">resultInfo</span></span>                     | [<span data-ttu-id="bd272-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="bd272-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="bd272-122">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="bd272-122">The result information.</span></span>  <span data-ttu-id="bd272-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd272-123">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="bd272-124">status</span><span class="sxs-lookup"><span data-stu-id="bd272-124">status</span></span>                         | <span data-ttu-id="bd272-125">String</span><span class="sxs-lookup"><span data-stu-id="bd272-125">String</span></span>                      | <span data-ttu-id="bd272-126">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="bd272-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="bd272-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd272-127">Read-only.</span></span>                                                  |

## <a name="relationships"></a><span data-ttu-id="bd272-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="bd272-128">Relationships</span></span>
<span data-ttu-id="bd272-129">Нет</span><span class="sxs-lookup"><span data-stu-id="bd272-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd272-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd272-130">JSON representation</span></span>

<span data-ttu-id="bd272-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd272-131">The following is a JSON representation of the resource.</span></span>

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
