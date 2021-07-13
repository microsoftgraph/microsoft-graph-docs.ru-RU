---
title: тип ресурсов managementTemplateDetailedInfo
description: Представляет подробные сведения для шаблона управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e98d2ca41bc972a5dca33c575363b1bac27d87a5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403096"
---
# <a name="managementtemplatedetailedinfo-resource-type"></a><span data-ttu-id="72b44-103">тип ресурсов managementTemplateDetailedInfo</span><span class="sxs-lookup"><span data-stu-id="72b44-103">managementTemplateDetailedInfo resource type</span></span>

<span data-ttu-id="72b44-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="72b44-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b44-105">Представляет подробные сведения для шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="72b44-105">Represents detailed information for the management template.</span></span>

## <a name="properties"></a><span data-ttu-id="72b44-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="72b44-106">Properties</span></span>
|<span data-ttu-id="72b44-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="72b44-107">Property</span></span>|<span data-ttu-id="72b44-108">Тип</span><span class="sxs-lookup"><span data-stu-id="72b44-108">Type</span></span>|<span data-ttu-id="72b44-109">Описание</span><span class="sxs-lookup"><span data-stu-id="72b44-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72b44-110">category</span><span class="sxs-lookup"><span data-stu-id="72b44-110">category</span></span>|<span data-ttu-id="72b44-111">managementCategory</span><span class="sxs-lookup"><span data-stu-id="72b44-111">managementCategory</span></span>|<span data-ttu-id="72b44-112">Категория управления для шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="72b44-112">The management category for the management template.</span></span> <span data-ttu-id="72b44-113">Возможные значения: `custom`, `devices`, `identity`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="72b44-113">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="72b44-114">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72b44-114">Required.</span></span> <span data-ttu-id="72b44-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72b44-115">Read-only.</span></span>|
|<span data-ttu-id="72b44-116">displayName</span><span class="sxs-lookup"><span data-stu-id="72b44-116">displayName</span></span>|<span data-ttu-id="72b44-117">String</span><span class="sxs-lookup"><span data-stu-id="72b44-117">String</span></span>|<span data-ttu-id="72b44-118">Имя отображения шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="72b44-118">The display name for the management template.</span></span> <span data-ttu-id="72b44-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72b44-119">Required.</span></span> <span data-ttu-id="72b44-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72b44-120">Read-only.</span></span>|
|<span data-ttu-id="72b44-121">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="72b44-121">managementTemplateId</span></span>|<span data-ttu-id="72b44-122">String</span><span class="sxs-lookup"><span data-stu-id="72b44-122">String</span></span>|<span data-ttu-id="72b44-123">Уникальный идентификатор шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="72b44-123">The unique identifier for the management template.</span></span> <span data-ttu-id="72b44-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72b44-124">Required.</span></span> <span data-ttu-id="72b44-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72b44-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72b44-126">Связи</span><span class="sxs-lookup"><span data-stu-id="72b44-126">Relationships</span></span>
<span data-ttu-id="72b44-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72b44-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72b44-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="72b44-128">JSON representation</span></span>
<span data-ttu-id="72b44-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72b44-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateDetailedInfo",
  "managementTemplateId": "String",
  "displayName": "String",
  "category": "String"
}
```
