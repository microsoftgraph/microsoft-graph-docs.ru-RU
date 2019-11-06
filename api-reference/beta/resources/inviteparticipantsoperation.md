---
title: Тип ресурса ИнвитепартиЦипантсоператион
description: Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5802f5a8a63c971007cb6cda11f16823e6140298
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006685"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="595d3-103">Тип ресурса ИнвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="595d3-103">inviteParticipantsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="595d3-104">Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.</span><span class="sxs-lookup"><span data-stu-id="595d3-104">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="595d3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="595d3-105">Properties</span></span>

| <span data-ttu-id="595d3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="595d3-106">Property</span></span>                       | <span data-ttu-id="595d3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="595d3-107">Type</span></span>                        | <span data-ttu-id="595d3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="595d3-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="595d3-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="595d3-109">clientContext</span></span>                  | <span data-ttu-id="595d3-110">String</span><span class="sxs-lookup"><span data-stu-id="595d3-110">String</span></span>                      | <span data-ttu-id="595d3-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="595d3-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="595d3-112">id</span><span class="sxs-lookup"><span data-stu-id="595d3-112">id</span></span>                             | <span data-ttu-id="595d3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="595d3-113">String</span></span>                      | <span data-ttu-id="595d3-114">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="595d3-114">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="595d3-115">participants</span><span class="sxs-lookup"><span data-stu-id="595d3-115">participants</span></span> | <span data-ttu-id="595d3-116">Коллекция [инвитатионпартиЦипантинфо](invitationParticipantInfo.md)</span><span class="sxs-lookup"><span data-stu-id="595d3-116">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="595d3-117">Участники, которые необходимо пригласить.</span><span class="sxs-lookup"><span data-stu-id="595d3-117">The participants to invite.</span></span> |
| <span data-ttu-id="595d3-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="595d3-118">resultInfo</span></span>                     | [<span data-ttu-id="595d3-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="595d3-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="595d3-120">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="595d3-120">The result information.</span></span>  <span data-ttu-id="595d3-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="595d3-121">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="595d3-122">status</span><span class="sxs-lookup"><span data-stu-id="595d3-122">status</span></span>                         | <span data-ttu-id="595d3-123">String</span><span class="sxs-lookup"><span data-stu-id="595d3-123">String</span></span>                      | <span data-ttu-id="595d3-124">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="595d3-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="595d3-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="595d3-125">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="595d3-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="595d3-126">JSON representation</span></span>

<span data-ttu-id="595d3-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="595d3-127">The following is a JSON representation of the resource.</span></span>

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
