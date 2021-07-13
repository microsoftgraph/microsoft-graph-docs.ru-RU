---
title: тип ресурсов managementIntentInfo
description: Представляет сведения о связи для намерения управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 9bc58ff4c850661b968e7b540de9038074406ac5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402705"
---
# <a name="managementintentinfo-resource-type"></a><span data-ttu-id="f0555-103">тип ресурсов managementIntentInfo</span><span class="sxs-lookup"><span data-stu-id="f0555-103">managementIntentInfo resource type</span></span>

<span data-ttu-id="f0555-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f0555-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0555-105">Представляет сведения о связи для намерения управления.</span><span class="sxs-lookup"><span data-stu-id="f0555-105">Represents relationship information for a management intent.</span></span>

## <a name="properties"></a><span data-ttu-id="f0555-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0555-106">Properties</span></span>
|<span data-ttu-id="f0555-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0555-107">Property</span></span>|<span data-ttu-id="f0555-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f0555-108">Type</span></span>|<span data-ttu-id="f0555-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f0555-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0555-110">managementIntentDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0555-110">managementIntentDisplayName</span></span>|<span data-ttu-id="f0555-111">String</span><span class="sxs-lookup"><span data-stu-id="f0555-111">String</span></span>|<span data-ttu-id="f0555-112">Имя отображения для намерения управления.</span><span class="sxs-lookup"><span data-stu-id="f0555-112">The display name for the management intent.</span></span> <span data-ttu-id="f0555-113">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f0555-113">Optional.</span></span> <span data-ttu-id="f0555-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0555-114">Read-only.</span></span>|
|<span data-ttu-id="f0555-115">managementIntentId</span><span class="sxs-lookup"><span data-stu-id="f0555-115">managementIntentId</span></span>|<span data-ttu-id="f0555-116">String</span><span class="sxs-lookup"><span data-stu-id="f0555-116">String</span></span>|<span data-ttu-id="f0555-117">Идентификатор для намерения управления.</span><span class="sxs-lookup"><span data-stu-id="f0555-117">The identifier for the management intent.</span></span> <span data-ttu-id="f0555-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0555-118">Required.</span></span> <span data-ttu-id="f0555-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0555-119">Read-only.</span></span>|
|<span data-ttu-id="f0555-120">managementTemplates</span><span class="sxs-lookup"><span data-stu-id="f0555-120">managementTemplates</span></span>|<span data-ttu-id="f0555-121">[коллекция microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md)</span><span class="sxs-lookup"><span data-stu-id="f0555-121">[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) collection</span></span>|<span data-ttu-id="f0555-122">Коллекция сведений о шаблонах управления, связанных с намерением управления.</span><span class="sxs-lookup"><span data-stu-id="f0555-122">The collection of management template information associated with the management intent.</span></span> <span data-ttu-id="f0555-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f0555-123">Optional.</span></span> <span data-ttu-id="f0555-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0555-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0555-125">Связи</span><span class="sxs-lookup"><span data-stu-id="f0555-125">Relationships</span></span>
<span data-ttu-id="f0555-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f0555-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0555-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f0555-127">JSON representation</span></span>
<span data-ttu-id="f0555-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0555-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntentInfo",
  "managementIntentId": "String",
  "managementIntentDisplayName": "String",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
