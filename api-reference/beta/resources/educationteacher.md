---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект `teacher`, который присутствует, когда значение параметра primaryRole для пользователя — .
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 17019d5ff5c2bc9614e934ef66d63e459371469a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510857"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="301f0-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="301f0-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="301f0-104">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="301f0-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="301f0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="301f0-105">Properties</span></span>
| <span data-ttu-id="301f0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="301f0-106">Property</span></span>     | <span data-ttu-id="301f0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="301f0-107">Type</span></span>   |<span data-ttu-id="301f0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="301f0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="301f0-109">externalId</span><span class="sxs-lookup"><span data-stu-id="301f0-109">externalId</span></span>|<span data-ttu-id="301f0-110">String</span><span class="sxs-lookup"><span data-stu-id="301f0-110">String</span></span>| <span data-ttu-id="301f0-111">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="301f0-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="301f0-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="301f0-112">teacherNumber</span></span>|<span data-ttu-id="301f0-113">String</span><span class="sxs-lookup"><span data-stu-id="301f0-113">String</span></span>|<span data-ttu-id="301f0-114">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="301f0-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="301f0-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="301f0-115">JSON representation</span></span>

<span data-ttu-id="301f0-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="301f0-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationteacher.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
