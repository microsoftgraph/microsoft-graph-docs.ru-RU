---
title: Тип ресурса Упдатерекордингстатусоператион
description: Описывает формат ответа действия обновления состояния записи.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: de1cf2578f699fde25d8863d12fcf4e262d78000
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962551"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="38b38-103">Тип ресурса Упдатерекордингстатусоператион</span><span class="sxs-lookup"><span data-stu-id="38b38-103">updateRecordingStatusOperation resource type</span></span>

<span data-ttu-id="38b38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38b38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38b38-105">Описывает формат ответа действия обновления состояния записи.</span><span class="sxs-lookup"><span data-stu-id="38b38-105">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="38b38-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="38b38-106">Properties</span></span>

| <span data-ttu-id="38b38-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="38b38-107">Property</span></span>            | <span data-ttu-id="38b38-108">Тип</span><span class="sxs-lookup"><span data-stu-id="38b38-108">Type</span></span>                        | <span data-ttu-id="38b38-109">Описание</span><span class="sxs-lookup"><span data-stu-id="38b38-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="38b38-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="38b38-110">clientContext</span></span>       | <span data-ttu-id="38b38-111">String</span><span class="sxs-lookup"><span data-stu-id="38b38-111">String</span></span>                      | <span data-ttu-id="38b38-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="38b38-112">Unique client context string.</span></span> <span data-ttu-id="38b38-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="38b38-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="38b38-114">id</span><span class="sxs-lookup"><span data-stu-id="38b38-114">id</span></span>                  | <span data-ttu-id="38b38-115">Строка</span><span class="sxs-lookup"><span data-stu-id="38b38-115">String</span></span>                      | <span data-ttu-id="38b38-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38b38-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="38b38-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="38b38-117">resultInfo</span></span>          | [<span data-ttu-id="38b38-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="38b38-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="38b38-119">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="38b38-119">The result information.</span></span> <span data-ttu-id="38b38-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38b38-120">Read-only.</span></span>                                                 |
| <span data-ttu-id="38b38-121">status</span><span class="sxs-lookup"><span data-stu-id="38b38-121">status</span></span>              | <span data-ttu-id="38b38-122">String</span><span class="sxs-lookup"><span data-stu-id="38b38-122">String</span></span>                      | <span data-ttu-id="38b38-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="38b38-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="38b38-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="38b38-124">Relationships</span></span>
<span data-ttu-id="38b38-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="38b38-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38b38-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="38b38-126">JSON representation</span></span>

<span data-ttu-id="38b38-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38b38-127">The following is a JSON representation of the resource.</span></span>

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
