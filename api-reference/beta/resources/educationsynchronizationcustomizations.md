---
title: Тип ресурса educationSynchronizationCustomizations
description: Содержит список сущностей для синхронизации и их настройки, при их наличии.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 3254915887afc1e6b0da0b3b6c44b59689219ab1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918191"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="c1542-103">Тип ресурса educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="c1542-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="c1542-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1542-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1542-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1542-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1542-106">Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), при их наличии.</span><span class="sxs-lookup"><span data-stu-id="c1542-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="c1542-107">**Примечание:** Настройка свойств для синхронизации не применяется к **studentEnrollment** и **teacherRoster** сущности.</span><span class="sxs-lookup"><span data-stu-id="c1542-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="c1542-108">Этот ресурс, принадлежит следующие поставщики данных:</span><span class="sxs-lookup"><span data-stu-id="c1542-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="c1542-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="c1542-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="c1542-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="c1542-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="c1542-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1542-111">Properties</span></span>

| <span data-ttu-id="c1542-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1542-112">Property</span></span> | <span data-ttu-id="c1542-113">Тип</span><span class="sxs-lookup"><span data-stu-id="c1542-113">Type</span></span> | <span data-ttu-id="c1542-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c1542-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c1542-115">**School**</span><span class="sxs-lookup"><span data-stu-id="c1542-115">**school**</span></span> | [<span data-ttu-id="c1542-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c1542-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c1542-117">Настройка для сущности school.</span><span class="sxs-lookup"><span data-stu-id="c1542-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="c1542-118">**section**</span><span class="sxs-lookup"><span data-stu-id="c1542-118">**section**</span></span> | [<span data-ttu-id="c1542-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c1542-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c1542-120">Настройка раздела сущности.</span><span class="sxs-lookup"><span data-stu-id="c1542-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="c1542-121">**student**</span><span class="sxs-lookup"><span data-stu-id="c1542-121">**student**</span></span> | [<span data-ttu-id="c1542-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c1542-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c1542-123">Настройка для учащихся сущности.</span><span class="sxs-lookup"><span data-stu-id="c1542-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="c1542-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="c1542-124">**teacher**</span></span> | [<span data-ttu-id="c1542-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c1542-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c1542-126">Настройка для преподавателей сущности.</span><span class="sxs-lookup"><span data-stu-id="c1542-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="c1542-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="c1542-127">**studentEnrollment**</span></span> | [<span data-ttu-id="c1542-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c1542-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="c1542-129">Настройка для регистрации учащихся.</span><span class="sxs-lookup"><span data-stu-id="c1542-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="c1542-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="c1542-130">**teacherRoster**</span></span> | [<span data-ttu-id="c1542-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="c1542-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="c1542-132">Настройка для преподавателей участников.</span><span class="sxs-lookup"><span data-stu-id="c1542-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c1542-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1542-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
