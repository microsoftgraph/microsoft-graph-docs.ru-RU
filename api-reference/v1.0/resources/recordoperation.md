---
title: Тип ресурса Рекордоператион
description: Этот тип ресурса содержит сведения, связанные с записью звука.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9424055d5669b9279dede18b6eb3773da47d9b19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533886"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="138d0-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="138d0-103">recordOperation resource type</span></span>

<span data-ttu-id="138d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="138d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="138d0-105">Этот тип ресурса содержит сведения, связанные с записью звука.</span><span class="sxs-lookup"><span data-stu-id="138d0-105">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="138d0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="138d0-106">Properties</span></span>

| <span data-ttu-id="138d0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="138d0-107">Property</span></span>                       | <span data-ttu-id="138d0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="138d0-108">Type</span></span>                        | <span data-ttu-id="138d0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="138d0-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="138d0-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="138d0-110">clientContext</span></span>                  | <span data-ttu-id="138d0-111">Строка</span><span class="sxs-lookup"><span data-stu-id="138d0-111">String</span></span>                      | <span data-ttu-id="138d0-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="138d0-112">Unique Client Context string.</span></span> <span data-ttu-id="138d0-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="138d0-113">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="138d0-114">id</span><span class="sxs-lookup"><span data-stu-id="138d0-114">id</span></span>                             | <span data-ttu-id="138d0-115">Строка</span><span class="sxs-lookup"><span data-stu-id="138d0-115">String</span></span>                      | <span data-ttu-id="138d0-116">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="138d0-116">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="138d0-117">рекордингакцесстокен</span><span class="sxs-lookup"><span data-stu-id="138d0-117">recordingAccessToken</span></span>           | <span data-ttu-id="138d0-118">Строка</span><span class="sxs-lookup"><span data-stu-id="138d0-118">String</span></span>                      | <span data-ttu-id="138d0-119">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="138d0-119">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="138d0-120">рекординглокатион</span><span class="sxs-lookup"><span data-stu-id="138d0-120">recordingLocation</span></span>              | <span data-ttu-id="138d0-121">Строка</span><span class="sxs-lookup"><span data-stu-id="138d0-121">String</span></span>                      | <span data-ttu-id="138d0-122">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="138d0-122">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="138d0-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="138d0-123">resultInfo</span></span>                     | [<span data-ttu-id="138d0-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="138d0-124">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="138d0-125">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="138d0-125">The result information.</span></span>  <span data-ttu-id="138d0-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="138d0-126">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="138d0-127">status</span><span class="sxs-lookup"><span data-stu-id="138d0-127">status</span></span>                         | <span data-ttu-id="138d0-128">String</span><span class="sxs-lookup"><span data-stu-id="138d0-128">String</span></span>                      | <span data-ttu-id="138d0-129">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="138d0-129">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="138d0-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="138d0-130">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="138d0-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="138d0-131">Relationships</span></span>
<span data-ttu-id="138d0-132">Нет</span><span class="sxs-lookup"><span data-stu-id="138d0-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="138d0-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="138d0-133">JSON representation</span></span>

<span data-ttu-id="138d0-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="138d0-134">The following is a JSON representation of the resource.</span></span>

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
