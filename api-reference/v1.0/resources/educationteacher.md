---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e2cfef452538b9b75500898bf9a809ee871d372
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030480"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="47376-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="47376-103">educationTeacher resource type</span></span>

<span data-ttu-id="47376-104">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="47376-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="47376-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="47376-105">Properties</span></span>
| <span data-ttu-id="47376-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="47376-106">Property</span></span>     | <span data-ttu-id="47376-107">Тип</span><span class="sxs-lookup"><span data-stu-id="47376-107">Type</span></span>   |<span data-ttu-id="47376-108">Описание</span><span class="sxs-lookup"><span data-stu-id="47376-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47376-109">externalId</span><span class="sxs-lookup"><span data-stu-id="47376-109">externalId</span></span>|<span data-ttu-id="47376-110">String</span><span class="sxs-lookup"><span data-stu-id="47376-110">String</span></span>| <span data-ttu-id="47376-111">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="47376-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="47376-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="47376-112">teacherNumber</span></span>|<span data-ttu-id="47376-113">String</span><span class="sxs-lookup"><span data-stu-id="47376-113">String</span></span>|<span data-ttu-id="47376-114">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="47376-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47376-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47376-115">JSON representation</span></span>

<span data-ttu-id="47376-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47376-116">The following is a JSON representation of the resource.</span></span>

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
