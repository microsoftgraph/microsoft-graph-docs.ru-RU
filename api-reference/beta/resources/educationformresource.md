---
title: Тип ресурса Едукатионформресаурце
description: Подкласс объекта Едукатионресаурце. Этот ресурс является формой.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d2e10ea6db0236b7deff3581c2e1b4f97c589045
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972721"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="2496c-104">Тип ресурса Едукатионформресаурце</span><span class="sxs-lookup"><span data-stu-id="2496c-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2496c-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="2496c-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="2496c-106">Этот ресурс является формой.</span><span class="sxs-lookup"><span data-stu-id="2496c-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="2496c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2496c-107">Properties</span></span>
| <span data-ttu-id="2496c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2496c-108">Property</span></span>     | <span data-ttu-id="2496c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2496c-109">Type</span></span>   |<span data-ttu-id="2496c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2496c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2496c-111">Оригиналформид</span><span class="sxs-lookup"><span data-stu-id="2496c-111">originalFormId</span></span>|<span data-ttu-id="2496c-112">String</span><span class="sxs-lookup"><span data-stu-id="2496c-112">String</span></span>|<span data-ttu-id="2496c-113">Исходный идентификатор формы.</span><span class="sxs-lookup"><span data-stu-id="2496c-113">Original id of the Form.</span></span>|
|<span data-ttu-id="2496c-114">Формид</span><span class="sxs-lookup"><span data-stu-id="2496c-114">formId</span></span>|<span data-ttu-id="2496c-115">String</span><span class="sxs-lookup"><span data-stu-id="2496c-115">String</span></span>|<span data-ttu-id="2496c-116">Идентификатор формы.</span><span class="sxs-lookup"><span data-stu-id="2496c-116">Id of the Form.</span></span>|
|<span data-ttu-id="2496c-117">Исграупформ</span><span class="sxs-lookup"><span data-stu-id="2496c-117">isGroupForm</span></span>|<span data-ttu-id="2496c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2496c-118">Boolean</span></span>|<span data-ttu-id="2496c-119">Принадлежность формы группе классов.</span><span class="sxs-lookup"><span data-stu-id="2496c-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="2496c-120">Виевурл</span><span class="sxs-lookup"><span data-stu-id="2496c-120">viewUrl</span></span>|<span data-ttu-id="2496c-121">String</span><span class="sxs-lookup"><span data-stu-id="2496c-121">String</span></span>|<span data-ttu-id="2496c-122">URL-адрес студента для формы.</span><span class="sxs-lookup"><span data-stu-id="2496c-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="2496c-123">Виевурл</span><span class="sxs-lookup"><span data-stu-id="2496c-123">viewUrl</span></span>|<span data-ttu-id="2496c-124">String</span><span class="sxs-lookup"><span data-stu-id="2496c-124">String</span></span>|<span data-ttu-id="2496c-125">URL-адрес студента для формы.</span><span class="sxs-lookup"><span data-stu-id="2496c-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="2496c-126">Едитурл</span><span class="sxs-lookup"><span data-stu-id="2496c-126">editUrl</span></span>|<span data-ttu-id="2496c-127">String</span><span class="sxs-lookup"><span data-stu-id="2496c-127">String</span></span>|<span data-ttu-id="2496c-128">URL-адрес преподавателя для формы.</span><span class="sxs-lookup"><span data-stu-id="2496c-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2496c-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2496c-129">JSON representation</span></span>

<span data-ttu-id="2496c-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2496c-130">The following is a JSON representation of the resource.</span></span>

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
