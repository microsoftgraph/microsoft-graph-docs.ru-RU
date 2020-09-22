---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 516322bd57dd29b8e9cd42c3662e173d4a4100fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032621"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="345ec-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="345ec-103">educationTeacher resource type</span></span>

<span data-ttu-id="345ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="345ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="345ec-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="345ec-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="345ec-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="345ec-106">Properties</span></span>
| <span data-ttu-id="345ec-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="345ec-107">Property</span></span>     | <span data-ttu-id="345ec-108">Тип</span><span class="sxs-lookup"><span data-stu-id="345ec-108">Type</span></span>   |<span data-ttu-id="345ec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="345ec-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="345ec-110">externalId</span><span class="sxs-lookup"><span data-stu-id="345ec-110">externalId</span></span>|<span data-ttu-id="345ec-111">String</span><span class="sxs-lookup"><span data-stu-id="345ec-111">String</span></span>| <span data-ttu-id="345ec-112">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="345ec-112">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="345ec-113">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="345ec-113">teacherNumber</span></span>|<span data-ttu-id="345ec-114">String</span><span class="sxs-lookup"><span data-stu-id="345ec-114">String</span></span>|<span data-ttu-id="345ec-115">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="345ec-115">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="345ec-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="345ec-116">JSON representation</span></span>

<span data-ttu-id="345ec-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="345ec-117">The following is a JSON representation of the resource.</span></span>

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

