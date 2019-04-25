---
title: Тип ресурса Едукатионформресаурце
description: Подкласс объекта Едукатионресаурце. Этот ресурс является формой.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5e0b03eeea8c0e9d22a9f7279c821f6d90211470
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542848"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="97854-104">Тип ресурса Едукатионформресаурце</span><span class="sxs-lookup"><span data-stu-id="97854-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97854-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="97854-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="97854-106">Этот ресурс является формой.</span><span class="sxs-lookup"><span data-stu-id="97854-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="97854-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="97854-107">Properties</span></span>
| <span data-ttu-id="97854-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="97854-108">Property</span></span>     | <span data-ttu-id="97854-109">Тип</span><span class="sxs-lookup"><span data-stu-id="97854-109">Type</span></span>   |<span data-ttu-id="97854-110">Описание</span><span class="sxs-lookup"><span data-stu-id="97854-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97854-111">Оригиналформид</span><span class="sxs-lookup"><span data-stu-id="97854-111">originalFormId</span></span>|<span data-ttu-id="97854-112">String</span><span class="sxs-lookup"><span data-stu-id="97854-112">String</span></span>|<span data-ttu-id="97854-113">Исходный идентификатор формы.</span><span class="sxs-lookup"><span data-stu-id="97854-113">Original id of the Form.</span></span>|
|<span data-ttu-id="97854-114">Формид</span><span class="sxs-lookup"><span data-stu-id="97854-114">formId</span></span>|<span data-ttu-id="97854-115">String</span><span class="sxs-lookup"><span data-stu-id="97854-115">String</span></span>|<span data-ttu-id="97854-116">Идентификатор формы.</span><span class="sxs-lookup"><span data-stu-id="97854-116">Id of the Form.</span></span>|
|<span data-ttu-id="97854-117">Исграупформ</span><span class="sxs-lookup"><span data-stu-id="97854-117">isGroupForm</span></span>|<span data-ttu-id="97854-118">Логический</span><span class="sxs-lookup"><span data-stu-id="97854-118">Boolean</span></span>|<span data-ttu-id="97854-119">Принадлежность формы группе классов.</span><span class="sxs-lookup"><span data-stu-id="97854-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="97854-120">Виевурл</span><span class="sxs-lookup"><span data-stu-id="97854-120">viewUrl</span></span>|<span data-ttu-id="97854-121">String</span><span class="sxs-lookup"><span data-stu-id="97854-121">String</span></span>|<span data-ttu-id="97854-122">URL-адрес студента для формы.</span><span class="sxs-lookup"><span data-stu-id="97854-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="97854-123">Виевурл</span><span class="sxs-lookup"><span data-stu-id="97854-123">viewUrl</span></span>|<span data-ttu-id="97854-124">String</span><span class="sxs-lookup"><span data-stu-id="97854-124">String</span></span>|<span data-ttu-id="97854-125">URL-адрес студента для формы.</span><span class="sxs-lookup"><span data-stu-id="97854-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="97854-126">Едитурл</span><span class="sxs-lookup"><span data-stu-id="97854-126">editUrl</span></span>|<span data-ttu-id="97854-127">String</span><span class="sxs-lookup"><span data-stu-id="97854-127">String</span></span>|<span data-ttu-id="97854-128">URL-адрес преподавателя для формы.</span><span class="sxs-lookup"><span data-stu-id="97854-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97854-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97854-129">JSON representation</span></span>

<span data-ttu-id="97854-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97854-130">The following is a JSON representation of the resource.</span></span>

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
