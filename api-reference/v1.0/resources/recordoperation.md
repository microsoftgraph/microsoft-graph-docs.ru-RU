---
title: Тип ресурса Рекордоператион
description: Этот тип ресурса содержит сведения, связанные с записью звука.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 508404a3360b2b59656dc31df6ec44f16f682cf4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991896"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="553cc-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="553cc-103">recordOperation resource type</span></span>

<span data-ttu-id="553cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="553cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="553cc-105">Этот тип ресурса содержит сведения, связанные с записью звука.</span><span class="sxs-lookup"><span data-stu-id="553cc-105">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="553cc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="553cc-106">Properties</span></span>

| <span data-ttu-id="553cc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="553cc-107">Property</span></span>                       | <span data-ttu-id="553cc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="553cc-108">Type</span></span>                        | <span data-ttu-id="553cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="553cc-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="553cc-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="553cc-110">clientContext</span></span>                  | <span data-ttu-id="553cc-111">String</span><span class="sxs-lookup"><span data-stu-id="553cc-111">String</span></span>                      | <span data-ttu-id="553cc-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="553cc-112">Unique Client Context string.</span></span> <span data-ttu-id="553cc-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="553cc-113">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="553cc-114">id</span><span class="sxs-lookup"><span data-stu-id="553cc-114">id</span></span>                             | <span data-ttu-id="553cc-115">String</span><span class="sxs-lookup"><span data-stu-id="553cc-115">String</span></span>                      | <span data-ttu-id="553cc-116">Идентификатор операции сервера. только для чтения.</span><span class="sxs-lookup"><span data-stu-id="553cc-116">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="553cc-117">рекордингакцесстокен</span><span class="sxs-lookup"><span data-stu-id="553cc-117">recordingAccessToken</span></span>           | <span data-ttu-id="553cc-118">String</span><span class="sxs-lookup"><span data-stu-id="553cc-118">String</span></span>                      | <span data-ttu-id="553cc-119">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="553cc-119">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="553cc-120">рекординглокатион</span><span class="sxs-lookup"><span data-stu-id="553cc-120">recordingLocation</span></span>              | <span data-ttu-id="553cc-121">String</span><span class="sxs-lookup"><span data-stu-id="553cc-121">String</span></span>                      | <span data-ttu-id="553cc-122">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="553cc-122">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="553cc-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="553cc-123">resultInfo</span></span>                     | [<span data-ttu-id="553cc-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="553cc-124">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="553cc-125">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="553cc-125">The result information.</span></span>  <span data-ttu-id="553cc-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="553cc-126">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="553cc-127">status</span><span class="sxs-lookup"><span data-stu-id="553cc-127">status</span></span>                         | <span data-ttu-id="553cc-128">String</span><span class="sxs-lookup"><span data-stu-id="553cc-128">String</span></span>                      | <span data-ttu-id="553cc-129">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="553cc-129">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="553cc-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="553cc-130">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="553cc-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="553cc-131">Relationships</span></span>
<span data-ttu-id="553cc-132">Нет</span><span class="sxs-lookup"><span data-stu-id="553cc-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="553cc-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="553cc-133">JSON representation</span></span>

<span data-ttu-id="553cc-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="553cc-134">The following is a JSON representation of the resource.</span></span>

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

