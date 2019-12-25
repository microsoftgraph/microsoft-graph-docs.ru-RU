---
title: Тип ресурса Рекордоператион
description: Этот тип ресурса содержит сведения, связанные с записью звука.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b4f0a62204a6ee1db7e75caf9044288f705a5529
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866256"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="0e0c2-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="0e0c2-103">recordOperation resource type</span></span>

<span data-ttu-id="0e0c2-104">Этот тип ресурса содержит сведения, связанные с записью звука.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-104">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="0e0c2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e0c2-105">Properties</span></span>

| <span data-ttu-id="0e0c2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e0c2-106">Property</span></span>                       | <span data-ttu-id="0e0c2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0e0c2-107">Type</span></span>                        | <span data-ttu-id="0e0c2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0e0c2-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0e0c2-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="0e0c2-109">clientContext</span></span>                  | <span data-ttu-id="0e0c2-110">String</span><span class="sxs-lookup"><span data-stu-id="0e0c2-110">String</span></span>                      | <span data-ttu-id="0e0c2-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-111">Unique Client Context string.</span></span> <span data-ttu-id="0e0c2-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="0e0c2-113">id</span><span class="sxs-lookup"><span data-stu-id="0e0c2-113">id</span></span>                             | <span data-ttu-id="0e0c2-114">Строка</span><span class="sxs-lookup"><span data-stu-id="0e0c2-114">String</span></span>                      | <span data-ttu-id="0e0c2-115">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="0e0c2-116">рекордингакцесстокен</span><span class="sxs-lookup"><span data-stu-id="0e0c2-116">recordingAccessToken</span></span>           | <span data-ttu-id="0e0c2-117">String</span><span class="sxs-lookup"><span data-stu-id="0e0c2-117">String</span></span>                      | <span data-ttu-id="0e0c2-118">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-118">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="0e0c2-119">рекординглокатион</span><span class="sxs-lookup"><span data-stu-id="0e0c2-119">recordingLocation</span></span>              | <span data-ttu-id="0e0c2-120">String</span><span class="sxs-lookup"><span data-stu-id="0e0c2-120">String</span></span>                      | <span data-ttu-id="0e0c2-121">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-121">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="0e0c2-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0e0c2-122">resultInfo</span></span>                     | [<span data-ttu-id="0e0c2-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0e0c2-123">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="0e0c2-124">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-124">The result information.</span></span>  <span data-ttu-id="0e0c2-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-125">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="0e0c2-126">status</span><span class="sxs-lookup"><span data-stu-id="0e0c2-126">status</span></span>                         | <span data-ttu-id="0e0c2-127">String</span><span class="sxs-lookup"><span data-stu-id="0e0c2-127">String</span></span>                      | <span data-ttu-id="0e0c2-128">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-128">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="0e0c2-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-129">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="0e0c2-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="0e0c2-130">Relationships</span></span>
<span data-ttu-id="0e0c2-131">Нет</span><span class="sxs-lookup"><span data-stu-id="0e0c2-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e0c2-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e0c2-132">JSON representation</span></span>

<span data-ttu-id="0e0c2-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e0c2-133">The following is a JSON representation of the resource.</span></span>

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
