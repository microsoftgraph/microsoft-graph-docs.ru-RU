---
title: Тип ресурса Упдатерекордингстатусоператион
description: Описывает формат ответа действия обновления состояния записи.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b27aca68e159775bc9e4559d1ff6d5c005c9929a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519591"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="b07ba-103">Тип ресурса Упдатерекордингстатусоператион</span><span class="sxs-lookup"><span data-stu-id="b07ba-103">updateRecordingStatusOperation resource type</span></span>

<span data-ttu-id="b07ba-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b07ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b07ba-105">Описывает формат ответа действия обновления состояния записи.</span><span class="sxs-lookup"><span data-stu-id="b07ba-105">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="b07ba-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b07ba-106">Properties</span></span>

| <span data-ttu-id="b07ba-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b07ba-107">Property</span></span>            | <span data-ttu-id="b07ba-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b07ba-108">Type</span></span>                        | <span data-ttu-id="b07ba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b07ba-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="b07ba-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="b07ba-110">clientContext</span></span>       | <span data-ttu-id="b07ba-111">String</span><span class="sxs-lookup"><span data-stu-id="b07ba-111">String</span></span>                      | <span data-ttu-id="b07ba-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="b07ba-112">Unique Client Context string.</span></span> <span data-ttu-id="b07ba-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="b07ba-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="b07ba-114">id</span><span class="sxs-lookup"><span data-stu-id="b07ba-114">id</span></span>                  | <span data-ttu-id="b07ba-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b07ba-115">String</span></span>                      | <span data-ttu-id="b07ba-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b07ba-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="b07ba-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b07ba-117">resultInfo</span></span>          | [<span data-ttu-id="b07ba-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b07ba-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b07ba-119">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="b07ba-119">The result information.</span></span> <span data-ttu-id="b07ba-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b07ba-120">Read-only.</span></span>                                                 |
| <span data-ttu-id="b07ba-121">status</span><span class="sxs-lookup"><span data-stu-id="b07ba-121">status</span></span>              | <span data-ttu-id="b07ba-122">String</span><span class="sxs-lookup"><span data-stu-id="b07ba-122">String</span></span>                      | <span data-ttu-id="b07ba-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b07ba-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="b07ba-124">Связи</span><span class="sxs-lookup"><span data-stu-id="b07ba-124">Relationships</span></span>
<span data-ttu-id="b07ba-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b07ba-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b07ba-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b07ba-126">JSON representation</span></span>

<span data-ttu-id="b07ba-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b07ba-127">The following is a JSON representation of the resource.</span></span>

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
