---
title: Тип ресурса educationSynchronizationCustomizations
description: Содержит список сущностей для синхронизации и их настройки, при их наличии.
localization_priority: Normal
ms.openlocfilehash: 0c07b166c09b2bfa6bf88159533523dab869a325
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817040"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="2e7ef-103">Тип ресурса educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="2e7ef-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="2e7ef-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e7ef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e7ef-106">Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), при их наличии.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="2e7ef-107">**Примечание:** Настройка свойств для синхронизации не применяется к **studentEnrollment** и **teacherRoster** сущности.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="2e7ef-108">Этот ресурс, принадлежит следующие поставщики данных:</span><span class="sxs-lookup"><span data-stu-id="2e7ef-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="2e7ef-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="2e7ef-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="2e7ef-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="2e7ef-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="2e7ef-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e7ef-111">Properties</span></span>

| <span data-ttu-id="2e7ef-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e7ef-112">Property</span></span> | <span data-ttu-id="2e7ef-113">Тип</span><span class="sxs-lookup"><span data-stu-id="2e7ef-113">Type</span></span> | <span data-ttu-id="2e7ef-114">Описание</span><span class="sxs-lookup"><span data-stu-id="2e7ef-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2e7ef-115">**School**</span><span class="sxs-lookup"><span data-stu-id="2e7ef-115">**school**</span></span> | [<span data-ttu-id="2e7ef-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="2e7ef-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="2e7ef-117">Настройка для сущности school.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="2e7ef-118">**section**</span><span class="sxs-lookup"><span data-stu-id="2e7ef-118">**section**</span></span> | [<span data-ttu-id="2e7ef-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="2e7ef-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="2e7ef-120">Настройка раздела сущности.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="2e7ef-121">**student**</span><span class="sxs-lookup"><span data-stu-id="2e7ef-121">**student**</span></span> | [<span data-ttu-id="2e7ef-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="2e7ef-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="2e7ef-123">Настройка для учащихся сущности.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="2e7ef-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="2e7ef-124">**teacher**</span></span> | [<span data-ttu-id="2e7ef-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="2e7ef-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="2e7ef-126">Настройка для преподавателей сущности.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="2e7ef-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="2e7ef-127">**studentEnrollment**</span></span> | [<span data-ttu-id="2e7ef-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="2e7ef-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="2e7ef-129">Настройка для регистрации учащихся.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="2e7ef-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="2e7ef-130">**teacherRoster**</span></span> | [<span data-ttu-id="2e7ef-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="2e7ef-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="2e7ef-132">Настройка для преподавателей участников.</span><span class="sxs-lookup"><span data-stu-id="2e7ef-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2e7ef-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e7ef-133">JSON representation</span></span>
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
