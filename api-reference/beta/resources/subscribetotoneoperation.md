---
title: Тип ресурса Субскрибетотонеоператион
description: Описывает формат ответа на создание подписки для получения тонов DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 824270ba51de4360084f9f978cab31b92730edc1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078166"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="0422d-103">Тип ресурса Субскрибетотонеоператион</span><span class="sxs-lookup"><span data-stu-id="0422d-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="0422d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0422d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0422d-105">Описывает формат ответа на создание подписки для получения тонов DTMF.</span><span class="sxs-lookup"><span data-stu-id="0422d-105">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="0422d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0422d-106">Properties</span></span>

| <span data-ttu-id="0422d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0422d-107">Property</span></span>                       | <span data-ttu-id="0422d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0422d-108">Type</span></span>                        | <span data-ttu-id="0422d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0422d-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0422d-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="0422d-110">clientContext</span></span>                  | <span data-ttu-id="0422d-111">String</span><span class="sxs-lookup"><span data-stu-id="0422d-111">String</span></span>                      | <span data-ttu-id="0422d-112">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="0422d-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="0422d-113">id</span><span class="sxs-lookup"><span data-stu-id="0422d-113">id</span></span>                             | <span data-ttu-id="0422d-114">String</span><span class="sxs-lookup"><span data-stu-id="0422d-114">String</span></span>                      | <span data-ttu-id="0422d-115">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="0422d-115">The server operation ID.</span></span> <span data-ttu-id="0422d-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0422d-116">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="0422d-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0422d-117">resultInfo</span></span>                     | [<span data-ttu-id="0422d-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0422d-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="0422d-119">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="0422d-119">The result information.</span></span>  <span data-ttu-id="0422d-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0422d-120">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="0422d-121">status</span><span class="sxs-lookup"><span data-stu-id="0422d-121">status</span></span>                         | <span data-ttu-id="0422d-122">String</span><span class="sxs-lookup"><span data-stu-id="0422d-122">String</span></span>                      | <span data-ttu-id="0422d-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0422d-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="0422d-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0422d-124">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="0422d-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="0422d-125">Relationships</span></span>
<span data-ttu-id="0422d-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0422d-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0422d-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0422d-127">JSON representation</span></span>

<span data-ttu-id="0422d-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0422d-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
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
  "description": "subscribeToToneOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


