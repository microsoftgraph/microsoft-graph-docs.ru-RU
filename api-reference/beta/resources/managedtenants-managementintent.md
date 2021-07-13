---
title: тип ресурсов managementIntent
description: Представляет метаданные для базового плана и какие шаблоны управления включены.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7648da23e5d49a9bd2910c2ccbde7e676a1d7cd0
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402706"
---
# <a name="managementintent-resource-type"></a><span data-ttu-id="46627-103">тип ресурсов managementIntent</span><span class="sxs-lookup"><span data-stu-id="46627-103">managementIntent resource type</span></span>

<span data-ttu-id="46627-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="46627-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46627-105">Представляет метаданные для базового плана и какие шаблоны управления включены.</span><span class="sxs-lookup"><span data-stu-id="46627-105">Represents metadata for a baseline and what management templates are included.</span></span>

## <a name="methods"></a><span data-ttu-id="46627-106">Методы</span><span class="sxs-lookup"><span data-stu-id="46627-106">Methods</span></span>
|<span data-ttu-id="46627-107">Метод</span><span class="sxs-lookup"><span data-stu-id="46627-107">Method</span></span>|<span data-ttu-id="46627-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="46627-108">Return type</span></span>|<span data-ttu-id="46627-109">Описание</span><span class="sxs-lookup"><span data-stu-id="46627-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="46627-110">Управление спискамиИнтенты</span><span class="sxs-lookup"><span data-stu-id="46627-110">List managementIntents</span></span>](../api/managedtenants-managedtenant-list-managementintents.md)|<span data-ttu-id="46627-111">[коллекция microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)</span><span class="sxs-lookup"><span data-stu-id="46627-111">[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md) collection</span></span>|<span data-ttu-id="46627-112">Получите список объектов [managementIntent](../resources/managedtenants-managementintent.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="46627-112">Get a list of the [managementIntent](../resources/managedtenants-managementintent.md) objects and their properties.</span></span>|
|[<span data-ttu-id="46627-113">Get managementIntent</span><span class="sxs-lookup"><span data-stu-id="46627-113">Get managementIntent</span></span>](../api/managedtenants-managementintent-get.md)|[<span data-ttu-id="46627-114">microsoft.graph.managedTenants.managementIntent</span><span class="sxs-lookup"><span data-stu-id="46627-114">microsoft.graph.managedTenants.managementIntent</span></span>](../resources/managedtenants-managementintent.md)|<span data-ttu-id="46627-115">Ознакомьтесь с свойствами и отношениями объекта [managementIntent.](../resources/managedtenants-managementintent.md)</span><span class="sxs-lookup"><span data-stu-id="46627-115">Read the properties and relationships of a [managementIntent](../resources/managedtenants-managementintent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="46627-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="46627-116">Properties</span></span>
|<span data-ttu-id="46627-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="46627-117">Property</span></span>|<span data-ttu-id="46627-118">Тип</span><span class="sxs-lookup"><span data-stu-id="46627-118">Type</span></span>|<span data-ttu-id="46627-119">Описание</span><span class="sxs-lookup"><span data-stu-id="46627-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46627-120">displayName</span><span class="sxs-lookup"><span data-stu-id="46627-120">displayName</span></span>|<span data-ttu-id="46627-121">String</span><span class="sxs-lookup"><span data-stu-id="46627-121">String</span></span>|<span data-ttu-id="46627-122">Имя отображения для намерения управления.</span><span class="sxs-lookup"><span data-stu-id="46627-122">The display name for the management intent.</span></span> <span data-ttu-id="46627-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="46627-123">Optional.</span></span> <span data-ttu-id="46627-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46627-124">Read-only.</span></span>|
|<span data-ttu-id="46627-125">id</span><span class="sxs-lookup"><span data-stu-id="46627-125">id</span></span>|<span data-ttu-id="46627-126">String</span><span class="sxs-lookup"><span data-stu-id="46627-126">String</span></span>|<span data-ttu-id="46627-127">Уникальный идентификатор для намерения управления.</span><span class="sxs-lookup"><span data-stu-id="46627-127">The unique identifier for the management intent.</span></span> <span data-ttu-id="46627-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46627-128">Required.</span></span> <span data-ttu-id="46627-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46627-129">Read-only.</span></span>|
|<span data-ttu-id="46627-130">isGlobal</span><span class="sxs-lookup"><span data-stu-id="46627-130">isGlobal</span></span>|<span data-ttu-id="46627-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="46627-131">Boolean</span></span>|<span data-ttu-id="46627-132">Флаг, указывающий, является ли намерение управления глобальным.</span><span class="sxs-lookup"><span data-stu-id="46627-132">A flag indicating whether the management intent is global.</span></span> <span data-ttu-id="46627-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46627-133">Required.</span></span> <span data-ttu-id="46627-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46627-134">Read-only.</span></span>|
|<span data-ttu-id="46627-135">managementTemplates</span><span class="sxs-lookup"><span data-stu-id="46627-135">managementTemplates</span></span>|<span data-ttu-id="46627-136">[коллекция microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md)</span><span class="sxs-lookup"><span data-stu-id="46627-136">[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) collection</span></span>|<span data-ttu-id="46627-137">Коллекция шаблонов управления, связанных с намерением управления.</span><span class="sxs-lookup"><span data-stu-id="46627-137">The collection of management templates associated with the management intent.</span></span> <span data-ttu-id="46627-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="46627-138">Optional.</span></span> <span data-ttu-id="46627-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46627-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46627-140">Связи</span><span class="sxs-lookup"><span data-stu-id="46627-140">Relationships</span></span>
<span data-ttu-id="46627-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="46627-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46627-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="46627-142">JSON representation</span></span>
<span data-ttu-id="46627-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46627-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementIntent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "isGlobal": "Boolean",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
