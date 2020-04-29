---
title: Тип ресурса ИнвитепартиЦипантсоператион
description: Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 54223a5b9e807dc45a9868b3251b8d8b1a0fcd72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447691"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="309fb-103">Тип ресурса ИнвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="309fb-103">inviteParticipantsOperation resource type</span></span>

<span data-ttu-id="309fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="309fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="309fb-105">Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.</span><span class="sxs-lookup"><span data-stu-id="309fb-105">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="309fb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="309fb-106">Properties</span></span>

| <span data-ttu-id="309fb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="309fb-107">Property</span></span>                       | <span data-ttu-id="309fb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="309fb-108">Type</span></span>                        | <span data-ttu-id="309fb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="309fb-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="309fb-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="309fb-110">clientContext</span></span>                  | <span data-ttu-id="309fb-111">String</span><span class="sxs-lookup"><span data-stu-id="309fb-111">String</span></span>                      | <span data-ttu-id="309fb-112">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="309fb-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="309fb-113">id</span><span class="sxs-lookup"><span data-stu-id="309fb-113">id</span></span>                             | <span data-ttu-id="309fb-114">Строка</span><span class="sxs-lookup"><span data-stu-id="309fb-114">String</span></span>                      | <span data-ttu-id="309fb-115">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="309fb-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="309fb-116">participants</span><span class="sxs-lookup"><span data-stu-id="309fb-116">participants</span></span> | <span data-ttu-id="309fb-117">Коллекция [invitationParticipantInfo](invitationParticipantInfo.md)</span><span class="sxs-lookup"><span data-stu-id="309fb-117">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="309fb-118">Участники, которые необходимо пригласить.</span><span class="sxs-lookup"><span data-stu-id="309fb-118">The participants to invite.</span></span> |
| <span data-ttu-id="309fb-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="309fb-119">resultInfo</span></span>                     | [<span data-ttu-id="309fb-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="309fb-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="309fb-121">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="309fb-121">The result information.</span></span>  <span data-ttu-id="309fb-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="309fb-122">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="309fb-123">status</span><span class="sxs-lookup"><span data-stu-id="309fb-123">status</span></span>                         | <span data-ttu-id="309fb-124">String</span><span class="sxs-lookup"><span data-stu-id="309fb-124">String</span></span>                      | <span data-ttu-id="309fb-125">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="309fb-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="309fb-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="309fb-126">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="309fb-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="309fb-127">JSON representation</span></span>

<span data-ttu-id="309fb-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="309fb-128">The following is a JSON representation of the resource.</span></span>

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
