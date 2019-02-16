---
title: Тип ресурса Аттендидатамодел
description: Тип участника.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8659b88cae8b9d2a94177593da40b61363fa23b
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057423"
---
# <a name="attendeedatamodel-resource-type"></a><span data-ttu-id="810d0-103">Тип ресурса Аттендидатамодел</span><span class="sxs-lookup"><span data-stu-id="810d0-103">attendeeDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="810d0-104">Представляет пользователя или ресурс, которые включаются в собрание.</span><span class="sxs-lookup"><span data-stu-id="810d0-104">Represents a person or resource who is being included in a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="810d0-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="810d0-105">JSON representation</span></span>

<span data-ttu-id="810d0-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="810d0-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "type"
  ],
  "@odata.type": "microsoft.graph.attendeeDataModel"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="810d0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="810d0-107">Properties</span></span>
| <span data-ttu-id="810d0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="810d0-108">Property</span></span>     | <span data-ttu-id="810d0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="810d0-109">Type</span></span>   |<span data-ttu-id="810d0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="810d0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="810d0-111">type</span><span class="sxs-lookup"><span data-stu-id="810d0-111">type</span></span>|<span data-ttu-id="810d0-112">attendeeType</span><span class="sxs-lookup"><span data-stu-id="810d0-112">attendeeType</span></span>| <span data-ttu-id="810d0-113">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="810d0-113">The type of attendee.</span></span> <span data-ttu-id="810d0-114">Возможные значения: `required`, `optional`,. `resource`</span><span class="sxs-lookup"><span data-stu-id="810d0-114">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="810d0-115">В настоящее время участником [findMeetingTimes](../api/user-findmeetingtimes.md) всегда считается, что этот человек относится к `required` типу.</span><span class="sxs-lookup"><span data-stu-id="810d0-115">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `required` type.</span></span>|
|<span data-ttu-id="810d0-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="810d0-116">emailAddress</span></span>|[<span data-ttu-id="810d0-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="810d0-117">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="810d0-118">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="810d0-118">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeedatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->