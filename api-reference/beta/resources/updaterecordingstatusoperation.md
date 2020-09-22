---
title: Тип ресурса Упдатерекордингстатусоператион
description: Описывает формат ответа действия обновления состояния записи.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 92c91d7e31f681e1d742c6a5354b4e221b4ebc6e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003488"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="66f3c-103">Тип ресурса Упдатерекордингстатусоператион</span><span class="sxs-lookup"><span data-stu-id="66f3c-103">updateRecordingStatusOperation resource type</span></span>

<span data-ttu-id="66f3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66f3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66f3c-105">Описывает формат ответа действия обновления состояния записи.</span><span class="sxs-lookup"><span data-stu-id="66f3c-105">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="66f3c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="66f3c-106">Properties</span></span>

| <span data-ttu-id="66f3c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="66f3c-107">Property</span></span>            | <span data-ttu-id="66f3c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="66f3c-108">Type</span></span>                        | <span data-ttu-id="66f3c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="66f3c-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="66f3c-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="66f3c-110">clientContext</span></span>       | <span data-ttu-id="66f3c-111">String</span><span class="sxs-lookup"><span data-stu-id="66f3c-111">String</span></span>                      | <span data-ttu-id="66f3c-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="66f3c-112">Unique Client Context string.</span></span> <span data-ttu-id="66f3c-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="66f3c-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="66f3c-114">id</span><span class="sxs-lookup"><span data-stu-id="66f3c-114">id</span></span>                  | <span data-ttu-id="66f3c-115">String</span><span class="sxs-lookup"><span data-stu-id="66f3c-115">String</span></span>                      | <span data-ttu-id="66f3c-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66f3c-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="66f3c-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="66f3c-117">resultInfo</span></span>          | [<span data-ttu-id="66f3c-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="66f3c-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="66f3c-119">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="66f3c-119">The result information.</span></span> <span data-ttu-id="66f3c-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66f3c-120">Read-only.</span></span>                                                 |
| <span data-ttu-id="66f3c-121">status</span><span class="sxs-lookup"><span data-stu-id="66f3c-121">status</span></span>              | <span data-ttu-id="66f3c-122">String</span><span class="sxs-lookup"><span data-stu-id="66f3c-122">String</span></span>                      | <span data-ttu-id="66f3c-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="66f3c-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="66f3c-124">Связи</span><span class="sxs-lookup"><span data-stu-id="66f3c-124">Relationships</span></span>
<span data-ttu-id="66f3c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="66f3c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66f3c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66f3c-126">JSON representation</span></span>

<span data-ttu-id="66f3c-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66f3c-127">The following is a JSON representation of the resource.</span></span>

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


