---
title: Тип ресурса ИнвитепартиЦипантсоператион
description: Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a974bd22ddd9e1ac8c6ab90cdedb9dda9f1a1bb5
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793037"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="dc489-103">Тип ресурса ИнвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="dc489-103">inviteParticipantsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc489-104">Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.</span><span class="sxs-lookup"><span data-stu-id="dc489-104">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="dc489-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc489-105">Properties</span></span>

| <span data-ttu-id="dc489-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc489-106">Property</span></span>                       | <span data-ttu-id="dc489-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dc489-107">Type</span></span>                        | <span data-ttu-id="dc489-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dc489-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="dc489-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="dc489-109">clientContext</span></span>                  | <span data-ttu-id="dc489-110">String.</span><span class="sxs-lookup"><span data-stu-id="dc489-110">String</span></span>                      | <span data-ttu-id="dc489-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="dc489-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="dc489-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc489-112">createdDateTime</span></span>                | <span data-ttu-id="dc489-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc489-113">DateTimeOffset</span></span>              | <span data-ttu-id="dc489-114">Время создания записи.</span><span class="sxs-lookup"><span data-stu-id="dc489-114">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="dc489-115">id</span><span class="sxs-lookup"><span data-stu-id="dc489-115">id</span></span>                             | <span data-ttu-id="dc489-116">Строка</span><span class="sxs-lookup"><span data-stu-id="dc489-116">String</span></span>                      | <span data-ttu-id="dc489-117">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc489-117">The server operation id. Read-only.</span></span> <span data-ttu-id="dc489-118">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="dc489-118">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="dc489-119">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="dc489-119">lastActionDateTime</span></span>             | <span data-ttu-id="dc489-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc489-120">DateTimeOffset</span></span>              | <span data-ttu-id="dc489-121">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="dc489-121">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="dc489-122">participants</span><span class="sxs-lookup"><span data-stu-id="dc489-122">participants</span></span> | <span data-ttu-id="dc489-123">Коллекция [инвитатионпартиЦипантинфо](invitationParticipantInfo.md)</span><span class="sxs-lookup"><span data-stu-id="dc489-123">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="dc489-124">Участники, которые необходимо пригласить.</span><span class="sxs-lookup"><span data-stu-id="dc489-124">The participants to invite.</span></span> |
| <span data-ttu-id="dc489-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="dc489-125">resultInfo</span></span>                     | [<span data-ttu-id="dc489-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="dc489-126">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="dc489-127">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="dc489-127">The result information.</span></span>  <span data-ttu-id="dc489-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc489-128">Read-only.</span></span> <span data-ttu-id="dc489-129">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="dc489-129">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="dc489-130">status</span><span class="sxs-lookup"><span data-stu-id="dc489-130">status</span></span>                         | <span data-ttu-id="dc489-131">String</span><span class="sxs-lookup"><span data-stu-id="dc489-131">String</span></span>                      | <span data-ttu-id="dc489-132">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="dc489-132">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="dc489-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc489-133">Read-only.</span></span> <span data-ttu-id="dc489-134">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="dc489-134">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="dc489-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="dc489-135">Relationships</span></span>
<span data-ttu-id="dc489-136">Нет</span><span class="sxs-lookup"><span data-stu-id="dc489-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc489-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc489-137">JSON representation</span></span>

<span data-ttu-id="dc489-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc489-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
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
