---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d31be9bd808f411c1e208ab953784fdefd65fdda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972441"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="376fc-103">Тип ресурса Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="376fc-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="376fc-104">Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), если они есть.</span><span class="sxs-lookup"><span data-stu-id="376fc-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="376fc-105">**Примечание:** Настройка свойств для синхронизации не применяется к объектам **студентенроллмент** и **теачерростер** .</span><span class="sxs-lookup"><span data-stu-id="376fc-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="376fc-106">Этот ресурс является членом следующих поставщиков данных:</span><span class="sxs-lookup"><span data-stu-id="376fc-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="376fc-107">Едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="376fc-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="376fc-108">Едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="376fc-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="376fc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="376fc-109">Properties</span></span>

| <span data-ttu-id="376fc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="376fc-110">Property</span></span> | <span data-ttu-id="376fc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="376fc-111">Type</span></span> | <span data-ttu-id="376fc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="376fc-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="376fc-113">**Название**</span><span class="sxs-lookup"><span data-stu-id="376fc-113">**school**</span></span> | [<span data-ttu-id="376fc-114">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="376fc-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="376fc-115">Настройка для учебного объекта School.</span><span class="sxs-lookup"><span data-stu-id="376fc-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="376fc-116">**section**</span><span class="sxs-lookup"><span data-stu-id="376fc-116">**section**</span></span> | [<span data-ttu-id="376fc-117">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="376fc-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="376fc-118">Настройка для объекта Section.</span><span class="sxs-lookup"><span data-stu-id="376fc-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="376fc-119">**student**</span><span class="sxs-lookup"><span data-stu-id="376fc-119">**student**</span></span> | [<span data-ttu-id="376fc-120">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="376fc-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="376fc-121">Настройка для объекта Student.</span><span class="sxs-lookup"><span data-stu-id="376fc-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="376fc-122">**teacher**</span><span class="sxs-lookup"><span data-stu-id="376fc-122">**teacher**</span></span> | [<span data-ttu-id="376fc-123">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="376fc-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="376fc-124">Настройка для объекта учителя.</span><span class="sxs-lookup"><span data-stu-id="376fc-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="376fc-125">**Студентенроллмент**</span><span class="sxs-lookup"><span data-stu-id="376fc-125">**studentEnrollment**</span></span> | [<span data-ttu-id="376fc-126">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="376fc-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="376fc-127">Настройка регистрации для учащихся.</span><span class="sxs-lookup"><span data-stu-id="376fc-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="376fc-128">**Теачерростер**</span><span class="sxs-lookup"><span data-stu-id="376fc-128">**teacherRoster**</span></span> | [<span data-ttu-id="376fc-129">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="376fc-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="376fc-130">Настройка для списка преподавателей.</span><span class="sxs-lookup"><span data-stu-id="376fc-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="376fc-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="376fc-131">JSON representation</span></span>
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
