---
title: Тип ресурса ИнвитепартиЦипантсоператион
description: Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 26a1b0574473ed540e28b72cd11fd6a10781452b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988998"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="e0e82-103">Тип ресурса ИнвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="e0e82-103">inviteParticipantsOperation resource type</span></span>

<span data-ttu-id="e0e82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0e82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0e82-105">Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.</span><span class="sxs-lookup"><span data-stu-id="e0e82-105">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="e0e82-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0e82-106">Properties</span></span>

| <span data-ttu-id="e0e82-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0e82-107">Property</span></span>                       | <span data-ttu-id="e0e82-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e0e82-108">Type</span></span>                        | <span data-ttu-id="e0e82-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e0e82-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e0e82-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="e0e82-110">clientContext</span></span>                  | <span data-ttu-id="e0e82-111">String</span><span class="sxs-lookup"><span data-stu-id="e0e82-111">String</span></span>                      | <span data-ttu-id="e0e82-112">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="e0e82-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="e0e82-113">id</span><span class="sxs-lookup"><span data-stu-id="e0e82-113">id</span></span>                             | <span data-ttu-id="e0e82-114">String</span><span class="sxs-lookup"><span data-stu-id="e0e82-114">String</span></span>                      | <span data-ttu-id="e0e82-115">Идентификатор операции сервера. только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e82-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="e0e82-116">participants</span><span class="sxs-lookup"><span data-stu-id="e0e82-116">participants</span></span> | <span data-ttu-id="e0e82-117">Коллекция [invitationParticipantInfo](invitationParticipantInfo.md)</span><span class="sxs-lookup"><span data-stu-id="e0e82-117">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="e0e82-118">Участники, которые необходимо пригласить.</span><span class="sxs-lookup"><span data-stu-id="e0e82-118">The participants to invite.</span></span> |
| <span data-ttu-id="e0e82-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e0e82-119">resultInfo</span></span>                     | [<span data-ttu-id="e0e82-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e0e82-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="e0e82-121">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="e0e82-121">The result information.</span></span>  <span data-ttu-id="e0e82-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e82-122">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="e0e82-123">status</span><span class="sxs-lookup"><span data-stu-id="e0e82-123">status</span></span>                         | <span data-ttu-id="e0e82-124">String</span><span class="sxs-lookup"><span data-stu-id="e0e82-124">String</span></span>                      | <span data-ttu-id="e0e82-125">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e0e82-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="e0e82-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e82-126">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="e0e82-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0e82-127">JSON representation</span></span>

<span data-ttu-id="e0e82-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0e82-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "participants": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inviteParticipantsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->


