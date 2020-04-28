---
title: Тип ресурса Едукатионассигнментграде
description: " Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9680a298c405a81648ba0a5fe95cdf0df0c841bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502748"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="cc692-103">Тип ресурса Едукатионассигнментграде</span><span class="sxs-lookup"><span data-stu-id="cc692-103">educationAssignmentGrade resource type</span></span>

<span data-ttu-id="cc692-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc692-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc692-105">Представляет объект **Grade** при отправке.</span><span class="sxs-lookup"><span data-stu-id="cc692-105">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="cc692-106">Это абстрактный тип, экземпляры которого никогда не будут создаваться; Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cc692-106">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="cc692-107">Кроме того, этот объект отслеживает круг пользователей, выполняющих ступенчатое выполнение.</span><span class="sxs-lookup"><span data-stu-id="cc692-107">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="cc692-108">Используется в свойстве **отсылки. Grade** .</span><span class="sxs-lookup"><span data-stu-id="cc692-108">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="cc692-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc692-109">Properties</span></span>
| <span data-ttu-id="cc692-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc692-110">Property</span></span>     | <span data-ttu-id="cc692-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cc692-111">Type</span></span>   |<span data-ttu-id="cc692-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cc692-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc692-113">градедби</span><span class="sxs-lookup"><span data-stu-id="cc692-113">gradedBy</span></span>|[<span data-ttu-id="cc692-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="cc692-114">identitySet</span></span>](identityset.md)| <span data-ttu-id="cc692-115">Пользователь, который выполнил ступенчатое.</span><span class="sxs-lookup"><span data-stu-id="cc692-115">User who did the grading.</span></span> |
|<span data-ttu-id="cc692-116">градеддатетиме</span><span class="sxs-lookup"><span data-stu-id="cc692-116">gradedDateTime</span></span>|<span data-ttu-id="cc692-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc692-117">DateTimeOffset</span></span>| <span data-ttu-id="cc692-118">Момент времени, когда уровень был применен к этому объекту отправки.</span><span class="sxs-lookup"><span data-stu-id="cc692-118">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="cc692-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="cc692-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc692-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cc692-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc692-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc692-121">JSON representation</span></span>

<span data-ttu-id="cc692-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc692-122">The following is a JSON representation of the resource.</span></span>

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
