---
title: Тип ресурса Едукатионассигнментграде
description: " Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: e925059a5eb06e5cc9795f78368b884fa40dd3ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334546"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="af32c-103">Тип ресурса Едукатионассигнментграде</span><span class="sxs-lookup"><span data-stu-id="af32c-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af32c-104">Представляет объект **Grade** при отправке.</span><span class="sxs-lookup"><span data-stu-id="af32c-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="af32c-105">Это абстрактный тип, экземпляры которого никогда не будут создаваться; Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="af32c-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="af32c-106">Кроме того, этот объект отслеживает круг пользователей, выполняющих ступенчатое выполнение.</span><span class="sxs-lookup"><span data-stu-id="af32c-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="af32c-107">Используется в свойстве **отсылки. Grade** .</span><span class="sxs-lookup"><span data-stu-id="af32c-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="af32c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="af32c-108">Properties</span></span>
| <span data-ttu-id="af32c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="af32c-109">Property</span></span>     | <span data-ttu-id="af32c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="af32c-110">Type</span></span>   |<span data-ttu-id="af32c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="af32c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af32c-112">Градедби</span><span class="sxs-lookup"><span data-stu-id="af32c-112">gradedBy</span></span>|[<span data-ttu-id="af32c-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="af32c-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="af32c-114">Пользователь, который выполнил ступенчатое.</span><span class="sxs-lookup"><span data-stu-id="af32c-114">User who did the grading.</span></span> |
|<span data-ttu-id="af32c-115">Градеддатетиме</span><span class="sxs-lookup"><span data-stu-id="af32c-115">gradedDateTime</span></span>|<span data-ttu-id="af32c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af32c-116">DateTimeOffset</span></span>| <span data-ttu-id="af32c-117">Момент времени, когда уровень был применен к этому объекту отправки.</span><span class="sxs-lookup"><span data-stu-id="af32c-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="af32c-118">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="af32c-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="af32c-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="af32c-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af32c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af32c-120">JSON representation</span></span>

<span data-ttu-id="af32c-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af32c-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
