---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 092d8fb9d7c358114159428d676ab1a21ea9d091
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333885"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="6617a-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="6617a-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6617a-104">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="6617a-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="6617a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6617a-105">Properties</span></span>
| <span data-ttu-id="6617a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6617a-106">Property</span></span>     | <span data-ttu-id="6617a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6617a-107">Type</span></span>   |<span data-ttu-id="6617a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6617a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6617a-109">externalId</span><span class="sxs-lookup"><span data-stu-id="6617a-109">externalId</span></span>|<span data-ttu-id="6617a-110">String</span><span class="sxs-lookup"><span data-stu-id="6617a-110">String</span></span>| <span data-ttu-id="6617a-111">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="6617a-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="6617a-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="6617a-112">teacherNumber</span></span>|<span data-ttu-id="6617a-113">String</span><span class="sxs-lookup"><span data-stu-id="6617a-113">String</span></span>|<span data-ttu-id="6617a-114">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="6617a-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6617a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6617a-115">JSON representation</span></span>

<span data-ttu-id="6617a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6617a-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
