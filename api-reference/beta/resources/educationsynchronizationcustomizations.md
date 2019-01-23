---
title: Тип ресурса educationSynchronizationCustomizations
description: Содержит список сущностей для синхронизации и их настройки, при их наличии.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 18b37276730286650e3fd75ad57a6b16e7917a04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425962"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="9ff96-103">Тип ресурса educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="9ff96-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="9ff96-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ff96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ff96-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ff96-106">Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), при их наличии.</span><span class="sxs-lookup"><span data-stu-id="9ff96-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="9ff96-107">**Примечание:** Настройка свойств для синхронизации не применяется к **studentEnrollment** и **teacherRoster** сущности.</span><span class="sxs-lookup"><span data-stu-id="9ff96-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="9ff96-108">Этот ресурс, принадлежит следующие поставщики данных:</span><span class="sxs-lookup"><span data-stu-id="9ff96-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="9ff96-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="9ff96-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="9ff96-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="9ff96-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="9ff96-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ff96-111">Properties</span></span>

| <span data-ttu-id="9ff96-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ff96-112">Property</span></span> | <span data-ttu-id="9ff96-113">Тип</span><span class="sxs-lookup"><span data-stu-id="9ff96-113">Type</span></span> | <span data-ttu-id="9ff96-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9ff96-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9ff96-115">**School**</span><span class="sxs-lookup"><span data-stu-id="9ff96-115">**school**</span></span> | [<span data-ttu-id="9ff96-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="9ff96-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="9ff96-117">Настройка для сущности school.</span><span class="sxs-lookup"><span data-stu-id="9ff96-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="9ff96-118">**section**</span><span class="sxs-lookup"><span data-stu-id="9ff96-118">**section**</span></span> | [<span data-ttu-id="9ff96-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="9ff96-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="9ff96-120">Настройка раздела сущности.</span><span class="sxs-lookup"><span data-stu-id="9ff96-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="9ff96-121">**student**</span><span class="sxs-lookup"><span data-stu-id="9ff96-121">**student**</span></span> | [<span data-ttu-id="9ff96-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="9ff96-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="9ff96-123">Настройка для учащихся сущности.</span><span class="sxs-lookup"><span data-stu-id="9ff96-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="9ff96-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="9ff96-124">**teacher**</span></span> | [<span data-ttu-id="9ff96-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="9ff96-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="9ff96-126">Настройка для преподавателей сущности.</span><span class="sxs-lookup"><span data-stu-id="9ff96-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="9ff96-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="9ff96-127">**studentEnrollment**</span></span> | [<span data-ttu-id="9ff96-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="9ff96-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="9ff96-129">Настройка для регистрации учащихся.</span><span class="sxs-lookup"><span data-stu-id="9ff96-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="9ff96-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="9ff96-130">**teacherRoster**</span></span> | [<span data-ttu-id="9ff96-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="9ff96-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="9ff96-132">Настройка для преподавателей участников.</span><span class="sxs-lookup"><span data-stu-id="9ff96-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="9ff96-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ff96-133">JSON representation</span></span>
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
