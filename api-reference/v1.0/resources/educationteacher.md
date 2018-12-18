---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
ms.openlocfilehash: a880c3908b70e0b9d7c580492f45183b8f15425d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334463"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="be705-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="be705-103">educationTeacher resource type</span></span>

<span data-ttu-id="be705-104">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="be705-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="be705-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="be705-105">Properties</span></span>
| <span data-ttu-id="be705-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="be705-106">Property</span></span>     | <span data-ttu-id="be705-107">Тип</span><span class="sxs-lookup"><span data-stu-id="be705-107">Type</span></span>   |<span data-ttu-id="be705-108">Описание</span><span class="sxs-lookup"><span data-stu-id="be705-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be705-109">externalId</span><span class="sxs-lookup"><span data-stu-id="be705-109">externalId</span></span>|<span data-ttu-id="be705-110">String</span><span class="sxs-lookup"><span data-stu-id="be705-110">String</span></span>| <span data-ttu-id="be705-111">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="be705-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="be705-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="be705-112">teacherNumber</span></span>|<span data-ttu-id="be705-113">String</span><span class="sxs-lookup"><span data-stu-id="be705-113">String</span></span>|<span data-ttu-id="be705-114">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="be705-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be705-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="be705-115">JSON representation</span></span>

<span data-ttu-id="be705-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be705-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->