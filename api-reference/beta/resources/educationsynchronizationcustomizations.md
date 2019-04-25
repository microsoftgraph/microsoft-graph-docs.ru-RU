---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543205"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="dcb50-103">Тип ресурса Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="dcb50-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcb50-104">Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), если они есть.</span><span class="sxs-lookup"><span data-stu-id="dcb50-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="dcb50-105">**Примечание:** Настройка свойств для синхронизации не применяется к объектам **студентенроллмент** и **теачерростер** .</span><span class="sxs-lookup"><span data-stu-id="dcb50-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="dcb50-106">Этот ресурс является членом следующих поставщиков данных:</span><span class="sxs-lookup"><span data-stu-id="dcb50-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="dcb50-107">Едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="dcb50-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="dcb50-108">Едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="dcb50-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="dcb50-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcb50-109">Properties</span></span>

| <span data-ttu-id="dcb50-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcb50-110">Property</span></span> | <span data-ttu-id="dcb50-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dcb50-111">Type</span></span> | <span data-ttu-id="dcb50-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb50-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="dcb50-113">**Название**</span><span class="sxs-lookup"><span data-stu-id="dcb50-113">**school**</span></span> | [<span data-ttu-id="dcb50-114">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="dcb50-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="dcb50-115">Настройка для учебного объекта School.</span><span class="sxs-lookup"><span data-stu-id="dcb50-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="dcb50-116">**section**</span><span class="sxs-lookup"><span data-stu-id="dcb50-116">**section**</span></span> | [<span data-ttu-id="dcb50-117">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="dcb50-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="dcb50-118">Настройка для объекта Section.</span><span class="sxs-lookup"><span data-stu-id="dcb50-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="dcb50-119">**student**</span><span class="sxs-lookup"><span data-stu-id="dcb50-119">**student**</span></span> | [<span data-ttu-id="dcb50-120">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="dcb50-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="dcb50-121">Настройка для объекта Student.</span><span class="sxs-lookup"><span data-stu-id="dcb50-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="dcb50-122">**teacher**</span><span class="sxs-lookup"><span data-stu-id="dcb50-122">**teacher**</span></span> | [<span data-ttu-id="dcb50-123">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="dcb50-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="dcb50-124">Настройка для объекта учителя.</span><span class="sxs-lookup"><span data-stu-id="dcb50-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="dcb50-125">**Студентенроллмент**</span><span class="sxs-lookup"><span data-stu-id="dcb50-125">**studentEnrollment**</span></span> | [<span data-ttu-id="dcb50-126">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="dcb50-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="dcb50-127">Настройка регистрации для учащихся.</span><span class="sxs-lookup"><span data-stu-id="dcb50-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="dcb50-128">**Теачерростер**</span><span class="sxs-lookup"><span data-stu-id="dcb50-128">**teacherRoster**</span></span> | [<span data-ttu-id="dcb50-129">Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="dcb50-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="dcb50-130">Настройка для списка преподавателей.</span><span class="sxs-lookup"><span data-stu-id="dcb50-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="dcb50-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcb50-131">JSON representation</span></span>
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
