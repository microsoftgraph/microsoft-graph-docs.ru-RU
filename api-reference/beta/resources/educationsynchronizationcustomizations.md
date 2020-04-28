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
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="75cfe-103">Тип ресурса Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="75cfe-103">educationSynchronizationCustomizations resource type</span></span>

<span data-ttu-id="75cfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75cfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75cfe-105">Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), если они есть.</span><span class="sxs-lookup"><span data-stu-id="75cfe-105">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="75cfe-106">**Примечание:** Настройка свойств для синхронизации не применяется к объектам **студентенроллмент** и **теачерростер** .</span><span class="sxs-lookup"><span data-stu-id="75cfe-106">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="75cfe-107">Этот ресурс является членом следующих поставщиков данных:</span><span class="sxs-lookup"><span data-stu-id="75cfe-107">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="75cfe-108">едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="75cfe-108">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="75cfe-109">едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="75cfe-109">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="75cfe-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="75cfe-110">Properties</span></span>

| <span data-ttu-id="75cfe-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="75cfe-111">Property</span></span> | <span data-ttu-id="75cfe-112">Тип</span><span class="sxs-lookup"><span data-stu-id="75cfe-112">Type</span></span> | <span data-ttu-id="75cfe-113">Описание</span><span class="sxs-lookup"><span data-stu-id="75cfe-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="75cfe-114">**Название**</span><span class="sxs-lookup"><span data-stu-id="75cfe-114">**school**</span></span> | [<span data-ttu-id="75cfe-115">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="75cfe-115">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="75cfe-116">Настройка для учебного объекта School.</span><span class="sxs-lookup"><span data-stu-id="75cfe-116">Customization for a school entity.</span></span>        |
| <span data-ttu-id="75cfe-117">**section**</span><span class="sxs-lookup"><span data-stu-id="75cfe-117">**section**</span></span> | [<span data-ttu-id="75cfe-118">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="75cfe-118">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="75cfe-119">Настройка для объекта Section.</span><span class="sxs-lookup"><span data-stu-id="75cfe-119">Customization for a section entity.</span></span>         |
| <span data-ttu-id="75cfe-120">**student**</span><span class="sxs-lookup"><span data-stu-id="75cfe-120">**student**</span></span> | [<span data-ttu-id="75cfe-121">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="75cfe-121">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="75cfe-122">Настройка для объекта Student.</span><span class="sxs-lookup"><span data-stu-id="75cfe-122">Customization for a student entity.</span></span>         |
| <span data-ttu-id="75cfe-123">**teacher**</span><span class="sxs-lookup"><span data-stu-id="75cfe-123">**teacher**</span></span> | [<span data-ttu-id="75cfe-124">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="75cfe-124">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="75cfe-125">Настройка для объекта учителя.</span><span class="sxs-lookup"><span data-stu-id="75cfe-125">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="75cfe-126">**студентенроллмент**</span><span class="sxs-lookup"><span data-stu-id="75cfe-126">**studentEnrollment**</span></span> | [<span data-ttu-id="75cfe-127">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="75cfe-127">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="75cfe-128">Настройка регистрации для учащихся.</span><span class="sxs-lookup"><span data-stu-id="75cfe-128">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="75cfe-129">**теачерростер**</span><span class="sxs-lookup"><span data-stu-id="75cfe-129">**teacherRoster**</span></span> | [<span data-ttu-id="75cfe-130">едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="75cfe-130">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="75cfe-131">Настройка для списка преподавателей.</span><span class="sxs-lookup"><span data-stu-id="75cfe-131">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="75cfe-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75cfe-132">JSON representation</span></span>
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
