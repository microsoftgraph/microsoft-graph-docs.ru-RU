---
title: Тип ресурса Рекордоператион
description: Этот тип ресурса содержит сведения, связанные с записью звука.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 03cdf594b04c75cd14b31dfbaef5894e8aacd19d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913669"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="1b8d8-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="1b8d8-103">recordOperation resource type</span></span>

<span data-ttu-id="1b8d8-104">Этот тип ресурса содержит сведения, связанные с записью звука.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-104">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="1b8d8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b8d8-105">Properties</span></span>

| <span data-ttu-id="1b8d8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b8d8-106">Property</span></span>                       | <span data-ttu-id="1b8d8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1b8d8-107">Type</span></span>                        | <span data-ttu-id="1b8d8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1b8d8-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1b8d8-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="1b8d8-109">clientContext</span></span>                  | <span data-ttu-id="1b8d8-110">String</span><span class="sxs-lookup"><span data-stu-id="1b8d8-110">String</span></span>                      | <span data-ttu-id="1b8d8-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-111">Unique Client Context string.</span></span> <span data-ttu-id="1b8d8-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="1b8d8-113">id</span><span class="sxs-lookup"><span data-stu-id="1b8d8-113">id</span></span>                             | <span data-ttu-id="1b8d8-114">Строка</span><span class="sxs-lookup"><span data-stu-id="1b8d8-114">String</span></span>                      | <span data-ttu-id="1b8d8-115">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="1b8d8-116">рекордингакцесстокен</span><span class="sxs-lookup"><span data-stu-id="1b8d8-116">recordingAccessToken</span></span>           | <span data-ttu-id="1b8d8-117">String</span><span class="sxs-lookup"><span data-stu-id="1b8d8-117">String</span></span>                      | <span data-ttu-id="1b8d8-118">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-118">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="1b8d8-119">рекординглокатион</span><span class="sxs-lookup"><span data-stu-id="1b8d8-119">recordingLocation</span></span>              | <span data-ttu-id="1b8d8-120">String</span><span class="sxs-lookup"><span data-stu-id="1b8d8-120">String</span></span>                      | <span data-ttu-id="1b8d8-121">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-121">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="1b8d8-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="1b8d8-122">resultInfo</span></span>                     | [<span data-ttu-id="1b8d8-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="1b8d8-123">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="1b8d8-124">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-124">The result information.</span></span>  <span data-ttu-id="1b8d8-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-125">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="1b8d8-126">status</span><span class="sxs-lookup"><span data-stu-id="1b8d8-126">status</span></span>                         | <span data-ttu-id="1b8d8-127">String</span><span class="sxs-lookup"><span data-stu-id="1b8d8-127">String</span></span>                      | <span data-ttu-id="1b8d8-128">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-128">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="1b8d8-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-129">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="1b8d8-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="1b8d8-130">Relationships</span></span>
<span data-ttu-id="1b8d8-131">Нет</span><span class="sxs-lookup"><span data-stu-id="1b8d8-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b8d8-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b8d8-132">JSON representation</span></span>

<span data-ttu-id="1b8d8-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
