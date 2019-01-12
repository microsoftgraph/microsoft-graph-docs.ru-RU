---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b58d74e6b53b1721a5139d050c7e89197b8721be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929559"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="4f00b-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="4f00b-103">educationTeacher resource type</span></span>

<span data-ttu-id="4f00b-104">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="4f00b-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="4f00b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f00b-105">Properties</span></span>
| <span data-ttu-id="4f00b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f00b-106">Property</span></span>     | <span data-ttu-id="4f00b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4f00b-107">Type</span></span>   |<span data-ttu-id="4f00b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4f00b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f00b-109">externalId</span><span class="sxs-lookup"><span data-stu-id="4f00b-109">externalId</span></span>|<span data-ttu-id="4f00b-110">String</span><span class="sxs-lookup"><span data-stu-id="4f00b-110">String</span></span>| <span data-ttu-id="4f00b-111">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="4f00b-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="4f00b-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="4f00b-112">teacherNumber</span></span>|<span data-ttu-id="4f00b-113">String</span><span class="sxs-lookup"><span data-stu-id="4f00b-113">String</span></span>|<span data-ttu-id="4f00b-114">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="4f00b-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f00b-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4f00b-115">JSON representation</span></span>

<span data-ttu-id="4f00b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f00b-116">The following is a JSON representation of the resource.</span></span>

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
