---
title: Тип ресурса Канцелмедиапроцессингоператион
description: Этот тип ресурса используется для описания формата ответа операции отмены обработки мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5962b3f5aed89c7f2c0b01be3f8b4a035ac463da
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319622"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="181b1-103">Тип ресурса Канцелмедиапроцессингоператион</span><span class="sxs-lookup"><span data-stu-id="181b1-103">CancelMediaProcessingOperation resource type</span></span>

<span data-ttu-id="181b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="181b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="181b1-105">Описывает формат ответа операции отмены обработки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="181b1-105">Describes the response format of the cancel media processing operation.</span></span>

## <a name="properties"></a><span data-ttu-id="181b1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="181b1-106">Properties</span></span>

| <span data-ttu-id="181b1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="181b1-107">Property</span></span>      | <span data-ttu-id="181b1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="181b1-108">Type</span></span>                        | <span data-ttu-id="181b1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="181b1-109">Description</span></span>                                                                     |
| :------------ | :-------------------------- | :------------------------------------------------------------------------------ |
| <span data-ttu-id="181b1-110">ко</span><span class="sxs-lookup"><span data-stu-id="181b1-110">all</span></span>           | <span data-ttu-id="181b1-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="181b1-111">Boolean</span></span>                     | <span data-ttu-id="181b1-112">Указывает, следует ли остановить все операции или текущие.</span><span class="sxs-lookup"><span data-stu-id="181b1-112">Indicates whether to stop all operations or current.</span></span>                            |
| <span data-ttu-id="181b1-113">Контекст</span><span class="sxs-lookup"><span data-stu-id="181b1-113">clientContext</span></span> | <span data-ttu-id="181b1-114">String</span><span class="sxs-lookup"><span data-stu-id="181b1-114">String</span></span>                      | <span data-ttu-id="181b1-115">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="181b1-115">The client context.</span></span>                                                             |
| <span data-ttu-id="181b1-116">id</span><span class="sxs-lookup"><span data-stu-id="181b1-116">id</span></span>            | <span data-ttu-id="181b1-117">String</span><span class="sxs-lookup"><span data-stu-id="181b1-117">String</span></span>                      | <span data-ttu-id="181b1-118">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="181b1-118">The server operation ID.</span></span> <span data-ttu-id="181b1-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="181b1-119">Read-only.</span></span>                                             |
| <span data-ttu-id="181b1-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="181b1-120">resultInfo</span></span>    | [<span data-ttu-id="181b1-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="181b1-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="181b1-122">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="181b1-122">The result information.</span></span>  <span data-ttu-id="181b1-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="181b1-123">Read-only.</span></span>                                             |
| <span data-ttu-id="181b1-124">status</span><span class="sxs-lookup"><span data-stu-id="181b1-124">status</span></span>        | <span data-ttu-id="181b1-125">String</span><span class="sxs-lookup"><span data-stu-id="181b1-125">String</span></span>                      | <span data-ttu-id="181b1-126">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="181b1-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="181b1-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="181b1-127">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="181b1-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="181b1-128">Relationships</span></span>
<span data-ttu-id="181b1-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="181b1-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="181b1-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="181b1-130">JSON representation</span></span>

<span data-ttu-id="181b1-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="181b1-131">The following is a JSON representation of the resource.</span></span>

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
