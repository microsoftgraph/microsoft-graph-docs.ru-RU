---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d3bfbec774b0ce5ff749e78b0057799501f432c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055598"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="de9e9-103">Тип ресурса Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="de9e9-103">educationSynchronizationCustomizations resource type</span></span>

<span data-ttu-id="de9e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de9e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de9e9-105">Содержит список сущностей для синхронизации и их настройки, если они есть.</span><span class="sxs-lookup"><span data-stu-id="de9e9-105">Contains the list of entities to sync and their customizations, if any.</span></span>

> [!NOTE]
> <span data-ttu-id="de9e9-106">Настройка свойств для синхронизации не относится к регистрационным спискам студентов или преподавателям.</span><span class="sxs-lookup"><span data-stu-id="de9e9-106">Customization of properties to sync does not apply to the Student Enrollments or  Teacher Rosters.</span></span>

<span data-ttu-id="de9e9-107">Этот ресурс является членом следующих поставщиков данных:</span><span class="sxs-lookup"><span data-stu-id="de9e9-107">This resource is member of the following data providers:</span></span>

- [<span data-ttu-id="de9e9-108">едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="de9e9-108">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
- [<span data-ttu-id="de9e9-109">едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="de9e9-109">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="de9e9-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="de9e9-110">Properties</span></span>

| <span data-ttu-id="de9e9-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="de9e9-111">Property</span></span>          | <span data-ttu-id="de9e9-112">Тип</span><span class="sxs-lookup"><span data-stu-id="de9e9-112">Type</span></span>                                    | <span data-ttu-id="de9e9-113">Описание</span><span class="sxs-lookup"><span data-stu-id="de9e9-113">Description</span></span>                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="de9e9-114">Название</span><span class="sxs-lookup"><span data-stu-id="de9e9-114">school</span></span>            | <span data-ttu-id="de9e9-115">[едукатионсинчронизатионкустомизатион]</span><span class="sxs-lookup"><span data-stu-id="de9e9-115">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="de9e9-116">Настройки для учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="de9e9-116">Customizations for School entities.</span></span>     |
| <span data-ttu-id="de9e9-117">section</span><span class="sxs-lookup"><span data-stu-id="de9e9-117">section</span></span>           | <span data-ttu-id="de9e9-118">[едукатионсинчронизатионкустомизатион]</span><span class="sxs-lookup"><span data-stu-id="de9e9-118">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="de9e9-119">Настройки для сущностей раздела.</span><span class="sxs-lookup"><span data-stu-id="de9e9-119">Customizations for Section entities.</span></span>    |
| <span data-ttu-id="de9e9-120">student</span><span class="sxs-lookup"><span data-stu-id="de9e9-120">student</span></span>           | <span data-ttu-id="de9e9-121">[едукатионсинчронизатионкустомизатион]</span><span class="sxs-lookup"><span data-stu-id="de9e9-121">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="de9e9-122">Настройки для сущностей учащихся.</span><span class="sxs-lookup"><span data-stu-id="de9e9-122">Customizations for Student entities.</span></span>    |
| <span data-ttu-id="de9e9-123">teacher</span><span class="sxs-lookup"><span data-stu-id="de9e9-123">teacher</span></span>           | <span data-ttu-id="de9e9-124">[едукатионсинчронизатионкустомизатион]</span><span class="sxs-lookup"><span data-stu-id="de9e9-124">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="de9e9-125">Настройки для сущностей преподавателей.</span><span class="sxs-lookup"><span data-stu-id="de9e9-125">Customizations for Teacher entities.</span></span>    |
| <span data-ttu-id="de9e9-126">студентенроллмент</span><span class="sxs-lookup"><span data-stu-id="de9e9-126">studentEnrollment</span></span> | <span data-ttu-id="de9e9-127">[едукатионсинчронизатионкустомизатион]</span><span class="sxs-lookup"><span data-stu-id="de9e9-127">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="de9e9-128">Настройки для регистрации учащихся.</span><span class="sxs-lookup"><span data-stu-id="de9e9-128">Customizations for Student Enrollments.</span></span> |
| <span data-ttu-id="de9e9-129">теачерростер</span><span class="sxs-lookup"><span data-stu-id="de9e9-129">teacherRoster</span></span>     | <span data-ttu-id="de9e9-130">[едукатионсинчронизатионкустомизатион]</span><span class="sxs-lookup"><span data-stu-id="de9e9-130">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="de9e9-131">Настройки для списков преподавателей.</span><span class="sxs-lookup"><span data-stu-id="de9e9-131">Customizations for Teacher Rosters.</span></span>     |

[едукатионсинчронизатионкустомизатион]: educationsynchronizationcustomization.md
[educationsynchronizationcustomization]: educationsynchronizationcustomization.md

## <a name="json-representation"></a><span data-ttu-id="de9e9-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de9e9-133">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  }
}
```


