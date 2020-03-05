---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a2ff93d6a91d522c5d1140035e278e9832332321
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500452"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="fad49-103">Тип ресурса Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="fad49-103">educationSynchronizationCustomizations resource type</span></span>

<span data-ttu-id="fad49-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fad49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fad49-105">Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), если они есть.</span><span class="sxs-lookup"><span data-stu-id="fad49-105">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="fad49-106">**Примечание:** Настройка свойств для синхронизации не применяется к объектам **студентенроллмент** и **теачерростер** .</span><span class="sxs-lookup"><span data-stu-id="fad49-106">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="fad49-107">Этот ресурс является членом следующих поставщиков данных:</span><span class="sxs-lookup"><span data-stu-id="fad49-107">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="fad49-108">едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="fad49-108">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="fad49-109">едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="fad49-109">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="fad49-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="fad49-110">Properties</span></span>

| <span data-ttu-id="fad49-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="fad49-111">Property</span></span> | <span data-ttu-id="fad49-112">Тип</span><span class="sxs-lookup"><span data-stu-id="fad49-112">Type</span></span> | <span data-ttu-id="fad49-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fad49-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fad49-114">**Название**</span><span class="sxs-lookup"><span data-stu-id="fad49-114">**school**</span></span> | [<span data-ttu-id="fad49-115">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="fad49-115">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="fad49-116">Настройка для учебного объекта School.</span><span class="sxs-lookup"><span data-stu-id="fad49-116">Customization for a school entity.</span></span>        |
| <span data-ttu-id="fad49-117">**section**</span><span class="sxs-lookup"><span data-stu-id="fad49-117">**section**</span></span> | [<span data-ttu-id="fad49-118">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="fad49-118">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="fad49-119">Настройка для объекта Section.</span><span class="sxs-lookup"><span data-stu-id="fad49-119">Customization for a section entity.</span></span>         |
| <span data-ttu-id="fad49-120">**student**</span><span class="sxs-lookup"><span data-stu-id="fad49-120">**student**</span></span> | [<span data-ttu-id="fad49-121">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="fad49-121">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="fad49-122">Настройка для объекта Student.</span><span class="sxs-lookup"><span data-stu-id="fad49-122">Customization for a student entity.</span></span>         |
| <span data-ttu-id="fad49-123">**teacher**</span><span class="sxs-lookup"><span data-stu-id="fad49-123">**teacher**</span></span> | [<span data-ttu-id="fad49-124">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="fad49-124">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="fad49-125">Настройка для объекта учителя.</span><span class="sxs-lookup"><span data-stu-id="fad49-125">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="fad49-126">**студентенроллмент**</span><span class="sxs-lookup"><span data-stu-id="fad49-126">**studentEnrollment**</span></span> | [<span data-ttu-id="fad49-127">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="fad49-127">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="fad49-128">Настройка регистрации для учащихся.</span><span class="sxs-lookup"><span data-stu-id="fad49-128">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="fad49-129">**теачерростер**</span><span class="sxs-lookup"><span data-stu-id="fad49-129">**teacherRoster**</span></span> | [<span data-ttu-id="fad49-130">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="fad49-130">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="fad49-131">Настройка для списка преподавателей.</span><span class="sxs-lookup"><span data-stu-id="fad49-131">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="fad49-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fad49-132">JSON representation</span></span>
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
