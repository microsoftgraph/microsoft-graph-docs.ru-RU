---
title: Тип ресурса Едукатионассигнментграде
description: " Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41e981d268718a94e6b28df6b43c4c2f931b7ad2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013757"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="a7047-103">Тип ресурса Едукатионассигнментграде</span><span class="sxs-lookup"><span data-stu-id="a7047-103">educationAssignmentGrade resource type</span></span>

<span data-ttu-id="a7047-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7047-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7047-105">Представляет объект **Grade** при отправке.</span><span class="sxs-lookup"><span data-stu-id="a7047-105">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="a7047-106">Это абстрактный тип, экземпляры которого никогда не будут создаваться; Тем не менее, все типы ступенчатого (точки, проход/завершение и т. д.) являются подклассами этого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a7047-106">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="a7047-107">Кроме того, этот объект отслеживает круг пользователей, выполняющих ступенчатое выполнение.</span><span class="sxs-lookup"><span data-stu-id="a7047-107">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="a7047-108">Используется в свойстве **отсылки. Grade** .</span><span class="sxs-lookup"><span data-stu-id="a7047-108">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="a7047-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7047-109">Properties</span></span>
| <span data-ttu-id="a7047-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7047-110">Property</span></span>     | <span data-ttu-id="a7047-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a7047-111">Type</span></span>   |<span data-ttu-id="a7047-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a7047-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7047-113">градедби</span><span class="sxs-lookup"><span data-stu-id="a7047-113">gradedBy</span></span>|[<span data-ttu-id="a7047-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="a7047-114">identitySet</span></span>](identityset.md)| <span data-ttu-id="a7047-115">Пользователь, который выполнил ступенчатое.</span><span class="sxs-lookup"><span data-stu-id="a7047-115">User who did the grading.</span></span> |
|<span data-ttu-id="a7047-116">градеддатетиме</span><span class="sxs-lookup"><span data-stu-id="a7047-116">gradedDateTime</span></span>|<span data-ttu-id="a7047-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7047-117">DateTimeOffset</span></span>| <span data-ttu-id="a7047-118">Момент времени, когда уровень был применен к этому объекту отправки.</span><span class="sxs-lookup"><span data-stu-id="a7047-118">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="a7047-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a7047-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a7047-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a7047-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7047-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7047-121">JSON representation</span></span>

<span data-ttu-id="a7047-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7047-122">The following is a JSON representation of the resource.</span></span>

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


