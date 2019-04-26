---
title: Тип ресурса Едукатионформресаурце
description: Подкласс объекта Едукатионресаурце. Этот ресурс является формой.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f2747d94c80732091db06294b26546afc567e03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334267"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="4ba68-104">Тип ресурса Едукатионформресаурце</span><span class="sxs-lookup"><span data-stu-id="4ba68-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ba68-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="4ba68-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="4ba68-106">Этот ресурс является формой.</span><span class="sxs-lookup"><span data-stu-id="4ba68-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="4ba68-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ba68-107">Properties</span></span>
| <span data-ttu-id="4ba68-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ba68-108">Property</span></span>     | <span data-ttu-id="4ba68-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ba68-109">Type</span></span>   |<span data-ttu-id="4ba68-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ba68-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ba68-111">Оригиналформид</span><span class="sxs-lookup"><span data-stu-id="4ba68-111">originalFormId</span></span>|<span data-ttu-id="4ba68-112">String</span><span class="sxs-lookup"><span data-stu-id="4ba68-112">String</span></span>|<span data-ttu-id="4ba68-113">Исходный идентификатор формы.</span><span class="sxs-lookup"><span data-stu-id="4ba68-113">Original id of the Form.</span></span>|
|<span data-ttu-id="4ba68-114">Формид</span><span class="sxs-lookup"><span data-stu-id="4ba68-114">formId</span></span>|<span data-ttu-id="4ba68-115">String</span><span class="sxs-lookup"><span data-stu-id="4ba68-115">String</span></span>|<span data-ttu-id="4ba68-116">Идентификатор формы.</span><span class="sxs-lookup"><span data-stu-id="4ba68-116">Id of the Form.</span></span>|
|<span data-ttu-id="4ba68-117">Исграупформ</span><span class="sxs-lookup"><span data-stu-id="4ba68-117">isGroupForm</span></span>|<span data-ttu-id="4ba68-118">Логический</span><span class="sxs-lookup"><span data-stu-id="4ba68-118">Boolean</span></span>|<span data-ttu-id="4ba68-119">Принадлежность формы группе классов.</span><span class="sxs-lookup"><span data-stu-id="4ba68-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="4ba68-120">Виевурл</span><span class="sxs-lookup"><span data-stu-id="4ba68-120">viewUrl</span></span>|<span data-ttu-id="4ba68-121">String</span><span class="sxs-lookup"><span data-stu-id="4ba68-121">String</span></span>|<span data-ttu-id="4ba68-122">URL-адрес студента для формы.</span><span class="sxs-lookup"><span data-stu-id="4ba68-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="4ba68-123">Виевурл</span><span class="sxs-lookup"><span data-stu-id="4ba68-123">viewUrl</span></span>|<span data-ttu-id="4ba68-124">String</span><span class="sxs-lookup"><span data-stu-id="4ba68-124">String</span></span>|<span data-ttu-id="4ba68-125">URL-адрес студента для формы.</span><span class="sxs-lookup"><span data-stu-id="4ba68-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="4ba68-126">Едитурл</span><span class="sxs-lookup"><span data-stu-id="4ba68-126">editUrl</span></span>|<span data-ttu-id="4ba68-127">String</span><span class="sxs-lookup"><span data-stu-id="4ba68-127">String</span></span>|<span data-ttu-id="4ba68-128">URL-адрес преподавателя для формы.</span><span class="sxs-lookup"><span data-stu-id="4ba68-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ba68-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ba68-129">JSON representation</span></span>

<span data-ttu-id="4ba68-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ba68-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String",
  "formId": "String",
  "isGroupForm": "Boolean",
  "viewUrl": "String",
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
  "suppressions": []
}
-->
