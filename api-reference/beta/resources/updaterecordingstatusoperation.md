---
title: Тип ресурса Упдатерекордингстатусоператион
description: Описывает формат ответа действия обновления состояния записи.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 302ea2c5ce0cfb54168bf936f8c6e5829e0867c7
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913284"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="61540-103">Тип ресурса Упдатерекордингстатусоператион</span><span class="sxs-lookup"><span data-stu-id="61540-103">updateRecordingStatusOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61540-104">Описывает формат ответа действия обновления состояния записи.</span><span class="sxs-lookup"><span data-stu-id="61540-104">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="61540-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="61540-105">Properties</span></span>

| <span data-ttu-id="61540-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="61540-106">Property</span></span>            | <span data-ttu-id="61540-107">Тип</span><span class="sxs-lookup"><span data-stu-id="61540-107">Type</span></span>                        | <span data-ttu-id="61540-108">Описание</span><span class="sxs-lookup"><span data-stu-id="61540-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="61540-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="61540-109">clientContext</span></span>       | <span data-ttu-id="61540-110">String</span><span class="sxs-lookup"><span data-stu-id="61540-110">String</span></span>                      | <span data-ttu-id="61540-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="61540-111">Unique Client Context string.</span></span> <span data-ttu-id="61540-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="61540-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="61540-113">id</span><span class="sxs-lookup"><span data-stu-id="61540-113">id</span></span>                  | <span data-ttu-id="61540-114">Строка</span><span class="sxs-lookup"><span data-stu-id="61540-114">String</span></span>                      | <span data-ttu-id="61540-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61540-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="61540-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="61540-116">resultInfo</span></span>          | [<span data-ttu-id="61540-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="61540-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="61540-118">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="61540-118">The result information.</span></span> <span data-ttu-id="61540-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61540-119">Read-only.</span></span>                                                 |
| <span data-ttu-id="61540-120">status</span><span class="sxs-lookup"><span data-stu-id="61540-120">status</span></span>              | <span data-ttu-id="61540-121">String</span><span class="sxs-lookup"><span data-stu-id="61540-121">String</span></span>                      | <span data-ttu-id="61540-122">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="61540-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="61540-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="61540-123">Relationships</span></span>
<span data-ttu-id="61540-124">Нет</span><span class="sxs-lookup"><span data-stu-id="61540-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61540-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61540-125">JSON representation</span></span>

<span data-ttu-id="61540-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61540-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
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
<!--
{
  "type": "#page.annotation",
  "description": "updateRecordingStatusOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
