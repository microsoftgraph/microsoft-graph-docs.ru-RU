---
title: Тип ресурса Канцелмедиапроцессингоператион
description: Этот тип ресурса используется для описания формата ответа операции отмены обработки мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8edbc7dcc770429fd4c1ccaf7bc3374d973cd2ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069220"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="82b46-103">Тип ресурса Канцелмедиапроцессингоператион</span><span class="sxs-lookup"><span data-stu-id="82b46-103">CancelMediaProcessingOperation resource type</span></span>

<span data-ttu-id="82b46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82b46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82b46-105">Описывает формат ответа операции отмены обработки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="82b46-105">Describes the response format of the cancel media processing operation.</span></span>

## <a name="properties"></a><span data-ttu-id="82b46-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="82b46-106">Properties</span></span>

| <span data-ttu-id="82b46-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="82b46-107">Property</span></span>      | <span data-ttu-id="82b46-108">Тип</span><span class="sxs-lookup"><span data-stu-id="82b46-108">Type</span></span>                        | <span data-ttu-id="82b46-109">Описание</span><span class="sxs-lookup"><span data-stu-id="82b46-109">Description</span></span>                                                                     |
| :------------ | :-------------------------- | :------------------------------------------------------------------------------ |
| <span data-ttu-id="82b46-110">ко</span><span class="sxs-lookup"><span data-stu-id="82b46-110">all</span></span>           | <span data-ttu-id="82b46-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b46-111">Boolean</span></span>                     | <span data-ttu-id="82b46-112">Указывает, следует ли остановить все операции или текущие.</span><span class="sxs-lookup"><span data-stu-id="82b46-112">Indicates whether to stop all operations or current.</span></span>                            |
| <span data-ttu-id="82b46-113">Контекст</span><span class="sxs-lookup"><span data-stu-id="82b46-113">clientContext</span></span> | <span data-ttu-id="82b46-114">Строка</span><span class="sxs-lookup"><span data-stu-id="82b46-114">String</span></span>                      | <span data-ttu-id="82b46-115">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="82b46-115">The client context.</span></span>                                                             |
| <span data-ttu-id="82b46-116">id</span><span class="sxs-lookup"><span data-stu-id="82b46-116">id</span></span>            | <span data-ttu-id="82b46-117">Строка</span><span class="sxs-lookup"><span data-stu-id="82b46-117">String</span></span>                      | <span data-ttu-id="82b46-118">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="82b46-118">The server operation ID.</span></span> <span data-ttu-id="82b46-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82b46-119">Read-only.</span></span>                                             |
| <span data-ttu-id="82b46-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="82b46-120">resultInfo</span></span>    | [<span data-ttu-id="82b46-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="82b46-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="82b46-122">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="82b46-122">The result information.</span></span>  <span data-ttu-id="82b46-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82b46-123">Read-only.</span></span>                                             |
| <span data-ttu-id="82b46-124">status</span><span class="sxs-lookup"><span data-stu-id="82b46-124">status</span></span>        | <span data-ttu-id="82b46-125">String</span><span class="sxs-lookup"><span data-stu-id="82b46-125">String</span></span>                      | <span data-ttu-id="82b46-126">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="82b46-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="82b46-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82b46-127">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="82b46-128">Связи</span><span class="sxs-lookup"><span data-stu-id="82b46-128">Relationships</span></span>
<span data-ttu-id="82b46-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="82b46-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82b46-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="82b46-130">JSON representation</span></span>

<span data-ttu-id="82b46-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82b46-131">The following is a JSON representation of the resource.</span></span>

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

