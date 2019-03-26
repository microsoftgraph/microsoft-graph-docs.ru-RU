---
title: Тип ресурса Едукатионформресаурце
description: Подкласс объекта Едукатионресаурце. Этот ресурс является формой.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5e0b03eeea8c0e9d22a9f7279c821f6d90211470
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801041"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="74756-104">Тип ресурса Едукатионформресаурце</span><span class="sxs-lookup"><span data-stu-id="74756-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74756-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="74756-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="74756-106">Этот ресурс является формой.</span><span class="sxs-lookup"><span data-stu-id="74756-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="74756-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="74756-107">Properties</span></span>
| <span data-ttu-id="74756-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="74756-108">Property</span></span>     | <span data-ttu-id="74756-109">Тип</span><span class="sxs-lookup"><span data-stu-id="74756-109">Type</span></span>   |<span data-ttu-id="74756-110">Описание</span><span class="sxs-lookup"><span data-stu-id="74756-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74756-111">Оригиналформид</span><span class="sxs-lookup"><span data-stu-id="74756-111">originalFormId</span></span>|<span data-ttu-id="74756-112">String</span><span class="sxs-lookup"><span data-stu-id="74756-112">String</span></span>|<span data-ttu-id="74756-113">Исходный идентификатор формы.</span><span class="sxs-lookup"><span data-stu-id="74756-113">Original id of the Form.</span></span>|
|<span data-ttu-id="74756-114">Формид</span><span class="sxs-lookup"><span data-stu-id="74756-114">formId</span></span>|<span data-ttu-id="74756-115">String</span><span class="sxs-lookup"><span data-stu-id="74756-115">String</span></span>|<span data-ttu-id="74756-116">Идентификатор формы.</span><span class="sxs-lookup"><span data-stu-id="74756-116">Id of the Form.</span></span>|
|<span data-ttu-id="74756-117">Исграупформ</span><span class="sxs-lookup"><span data-stu-id="74756-117">isGroupForm</span></span>|<span data-ttu-id="74756-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="74756-118">Boolean</span></span>|<span data-ttu-id="74756-119">Принадлежность формы группе классов.</span><span class="sxs-lookup"><span data-stu-id="74756-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="74756-120">Виевурл</span><span class="sxs-lookup"><span data-stu-id="74756-120">viewUrl</span></span>|<span data-ttu-id="74756-121">String</span><span class="sxs-lookup"><span data-stu-id="74756-121">String</span></span>|<span data-ttu-id="74756-122">URL-адрес студента для формы.</span><span class="sxs-lookup"><span data-stu-id="74756-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="74756-123">Виевурл</span><span class="sxs-lookup"><span data-stu-id="74756-123">viewUrl</span></span>|<span data-ttu-id="74756-124">String</span><span class="sxs-lookup"><span data-stu-id="74756-124">String</span></span>|<span data-ttu-id="74756-125">URL-адрес студента для формы.</span><span class="sxs-lookup"><span data-stu-id="74756-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="74756-126">Едитурл</span><span class="sxs-lookup"><span data-stu-id="74756-126">editUrl</span></span>|<span data-ttu-id="74756-127">String</span><span class="sxs-lookup"><span data-stu-id="74756-127">String</span></span>|<span data-ttu-id="74756-128">URL-адрес преподавателя для формы.</span><span class="sxs-lookup"><span data-stu-id="74756-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74756-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74756-129">JSON representation</span></span>

<span data-ttu-id="74756-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74756-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String"
  "formId": "String"
  "isGroupForm": "Boolean"
  "viewUrl": "String"
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationformresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
