---
title: Тип ресурса educationSynchronizationCustomizations
description: Содержит список сущностей для синхронизации и их настройки, при их наличии.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523255"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="c66f9-103">Тип ресурса educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="c66f9-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c66f9-104">Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), при их наличии.</span><span class="sxs-lookup"><span data-stu-id="c66f9-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="c66f9-105">**Примечание:** Настройка свойств для синхронизации не применяется к **studentEnrollment** и **teacherRoster** сущности.</span><span class="sxs-lookup"><span data-stu-id="c66f9-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="c66f9-106">Этот ресурс, принадлежит следующие поставщики данных:</span><span class="sxs-lookup"><span data-stu-id="c66f9-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="c66f9-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="c66f9-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="c66f9-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="c66f9-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="c66f9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c66f9-109">Properties</span></span>

| <span data-ttu-id="c66f9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c66f9-110">Property</span></span> | <span data-ttu-id="c66f9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c66f9-111">Type</span></span> | <span data-ttu-id="c66f9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c66f9-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c66f9-113">**School**</span><span class="sxs-lookup"><span data-stu-id="c66f9-113">**school**</span></span> | [<span data-ttu-id="c66f9-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c66f9-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c66f9-115">Настройка для сущности school.</span><span class="sxs-lookup"><span data-stu-id="c66f9-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="c66f9-116">**section**</span><span class="sxs-lookup"><span data-stu-id="c66f9-116">**section**</span></span> | [<span data-ttu-id="c66f9-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c66f9-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c66f9-118">Настройка раздела сущности.</span><span class="sxs-lookup"><span data-stu-id="c66f9-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="c66f9-119">student</span><span class="sxs-lookup"><span data-stu-id="c66f9-119">**student**</span></span> | [<span data-ttu-id="c66f9-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c66f9-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c66f9-121">Настройка для учащихся сущности.</span><span class="sxs-lookup"><span data-stu-id="c66f9-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="c66f9-122">teacher</span><span class="sxs-lookup"><span data-stu-id="c66f9-122">**teacher**</span></span> | [<span data-ttu-id="c66f9-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c66f9-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c66f9-124">Настройка для преподавателей сущности.</span><span class="sxs-lookup"><span data-stu-id="c66f9-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="c66f9-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="c66f9-125">**studentEnrollment**</span></span> | [<span data-ttu-id="c66f9-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c66f9-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c66f9-127">Настройка для регистрации учащихся.</span><span class="sxs-lookup"><span data-stu-id="c66f9-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="c66f9-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="c66f9-128">**teacherRoster**</span></span> | [<span data-ttu-id="c66f9-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c66f9-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="c66f9-130">Настройка для преподавателей участников.</span><span class="sxs-lookup"><span data-stu-id="c66f9-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c66f9-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c66f9-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
