---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 494fc0d3bed992a8df4921fe8601024e7eb01668
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533003"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="ac73f-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="ac73f-103">educationTeacher resource type</span></span>

<span data-ttu-id="ac73f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac73f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac73f-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="ac73f-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="ac73f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac73f-106">Properties</span></span>
| <span data-ttu-id="ac73f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac73f-107">Property</span></span>     | <span data-ttu-id="ac73f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ac73f-108">Type</span></span>   |<span data-ttu-id="ac73f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ac73f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac73f-110">externalId</span><span class="sxs-lookup"><span data-stu-id="ac73f-110">externalId</span></span>|<span data-ttu-id="ac73f-111">Строка</span><span class="sxs-lookup"><span data-stu-id="ac73f-111">String</span></span>| <span data-ttu-id="ac73f-112">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="ac73f-112">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="ac73f-113">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="ac73f-113">teacherNumber</span></span>|<span data-ttu-id="ac73f-114">String</span><span class="sxs-lookup"><span data-stu-id="ac73f-114">String</span></span>|<span data-ttu-id="ac73f-115">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="ac73f-115">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac73f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac73f-116">JSON representation</span></span>

<span data-ttu-id="ac73f-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac73f-117">The following is a JSON representation of the resource.</span></span>

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
