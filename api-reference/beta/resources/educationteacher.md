---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
ms.openlocfilehash: ca174381fe8722c5b96848ced1d0e09b469068f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351662"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="c32be-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="c32be-103">educationTeacher resource type</span></span>

> <span data-ttu-id="c32be-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c32be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c32be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c32be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c32be-106">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="c32be-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="c32be-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c32be-107">Properties</span></span>
| <span data-ttu-id="c32be-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c32be-108">Property</span></span>     | <span data-ttu-id="c32be-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c32be-109">Type</span></span>   |<span data-ttu-id="c32be-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c32be-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c32be-111">externalId</span><span class="sxs-lookup"><span data-stu-id="c32be-111">externalId</span></span>|<span data-ttu-id="c32be-112">String</span><span class="sxs-lookup"><span data-stu-id="c32be-112">String</span></span>| <span data-ttu-id="c32be-113">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="c32be-113">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="c32be-114">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="c32be-114">teacherNumber</span></span>|<span data-ttu-id="c32be-115">String</span><span class="sxs-lookup"><span data-stu-id="c32be-115">String</span></span>|<span data-ttu-id="c32be-116">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="c32be-116">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c32be-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c32be-117">JSON representation</span></span>

<span data-ttu-id="c32be-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c32be-118">The following is a JSON representation of the resource.</span></span>

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