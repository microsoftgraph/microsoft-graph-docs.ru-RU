---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1bc49a3fbf494e378ec695af1f53c0ca4ea313ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521623"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="7451d-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="7451d-103">playPromptOperation resource type</span></span>

<span data-ttu-id="7451d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7451d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7451d-105">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="7451d-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="7451d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7451d-106">Properties</span></span>

| <span data-ttu-id="7451d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7451d-107">Property</span></span>            | <span data-ttu-id="7451d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7451d-108">Type</span></span>                        | <span data-ttu-id="7451d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7451d-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="7451d-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="7451d-110">clientContext</span></span>       | <span data-ttu-id="7451d-111">String</span><span class="sxs-lookup"><span data-stu-id="7451d-111">String</span></span>                      | <span data-ttu-id="7451d-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="7451d-112">Unique Client Context string.</span></span> <span data-ttu-id="7451d-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="7451d-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="7451d-114">комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="7451d-114">completionReason</span></span>    | <span data-ttu-id="7451d-115">String</span><span class="sxs-lookup"><span data-stu-id="7451d-115">String</span></span>                      | <span data-ttu-id="7451d-116">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="7451d-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="7451d-117">id</span><span class="sxs-lookup"><span data-stu-id="7451d-117">id</span></span>                  | <span data-ttu-id="7451d-118">Строка</span><span class="sxs-lookup"><span data-stu-id="7451d-118">String</span></span>                      | <span data-ttu-id="7451d-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7451d-119">Read-only.</span></span>                                                                         |
| <span data-ttu-id="7451d-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="7451d-120">resultInfo</span></span>          | [<span data-ttu-id="7451d-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="7451d-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="7451d-122">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="7451d-122">The result information.</span></span> <span data-ttu-id="7451d-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7451d-123">Read-only.</span></span>                                |
| <span data-ttu-id="7451d-124">status</span><span class="sxs-lookup"><span data-stu-id="7451d-124">status</span></span>              | <span data-ttu-id="7451d-125">String</span><span class="sxs-lookup"><span data-stu-id="7451d-125">String</span></span>                      | <span data-ttu-id="7451d-126">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7451d-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="7451d-127">Связи</span><span class="sxs-lookup"><span data-stu-id="7451d-127">Relationships</span></span>
<span data-ttu-id="7451d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="7451d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7451d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7451d-129">JSON representation</span></span>

<span data-ttu-id="7451d-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7451d-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
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
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
