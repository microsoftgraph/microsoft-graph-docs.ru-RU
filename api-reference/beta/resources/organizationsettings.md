---
title: Тип ресурса organizationSettings
description: Содержит параметры, применимые к организации или объектам-пользователям в ней.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 105a57c7cb5827e9017df7494d32802ef7ac6fa5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158326"
---
# <a name="organizationsettings-resource-type"></a><span data-ttu-id="af8c9-103">Тип ресурса organizationSettings</span><span class="sxs-lookup"><span data-stu-id="af8c9-103">organizationSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af8c9-104">Содержит параметры, применимые [](organization.md) к организации или применяемые к объектам [пользователей](user.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="af8c9-104">Contains settings that are applicable to the [organization](organization.md) or that should be applied to [user](user.md) objects within an organization.</span></span>

## <a name="methods"></a><span data-ttu-id="af8c9-105">Методы</span><span class="sxs-lookup"><span data-stu-id="af8c9-105">Methods</span></span>

| <span data-ttu-id="af8c9-106">Метод</span><span class="sxs-lookup"><span data-stu-id="af8c9-106">Method</span></span>       | <span data-ttu-id="af8c9-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="af8c9-107">Return Type</span></span> | <span data-ttu-id="af8c9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="af8c9-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="af8c9-109">Получить параметры организации</span><span class="sxs-lookup"><span data-stu-id="af8c9-109">Get organization settings</span></span>](../api/organizationsettings-get.md) | [<span data-ttu-id="af8c9-110">organizationSettings</span><span class="sxs-lookup"><span data-stu-id="af8c9-110">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="af8c9-111">Чтение объекта параметров организации.</span><span class="sxs-lookup"><span data-stu-id="af8c9-111">Read the organization settings object.</span></span> |
| [<span data-ttu-id="af8c9-112">Создание profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="af8c9-112">Create profileCardProperty</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="af8c9-113">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="af8c9-113">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="af8c9-114">Создание нового **объекта profileCardProperty** путем публикации в коллекции объектов **profileCardProperty.**</span><span class="sxs-lookup"><span data-stu-id="af8c9-114">Create a new **profileCardProperty** by posting to the **profileCardProperty** object collection.</span></span> |
| [<span data-ttu-id="af8c9-115">List profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="af8c9-115">List profileCardProperties</span></span>](../api/organizationsettings-list-profilecardproperties.md) | <span data-ttu-id="af8c9-116">[Коллекция profileCardProperty](profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="af8c9-116">[profileCardProperty](profilecardproperty.md) collection</span></span> | <span data-ttu-id="af8c9-117">Получите **коллекцию объектов profileCardProperty.**</span><span class="sxs-lookup"><span data-stu-id="af8c9-117">Get a **profileCardProperty** object collection.</span></span> |
| [<span data-ttu-id="af8c9-118">Get itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="af8c9-118">Get itemInsightsSettings</span></span>](../api/iteminsightssettings-get.md) | [<span data-ttu-id="af8c9-119">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="af8c9-119">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="af8c9-120">Получите свойства объекта **itemInsightsSettings.**</span><span class="sxs-lookup"><span data-stu-id="af8c9-120">Get the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="af8c9-121">Обновление itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="af8c9-121">Update itemInsightsSettings</span></span>](../api/iteminsightssettings-update.md) | [<span data-ttu-id="af8c9-122">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="af8c9-122">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="af8c9-123">Обновление свойств указанного ресурса **itemInsightsSettings.**</span><span class="sxs-lookup"><span data-stu-id="af8c9-123">Update the properties of the specified **itemInsightsSettings** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="af8c9-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="af8c9-124">Properties</span></span>

<span data-ttu-id="af8c9-125">Нет</span><span class="sxs-lookup"><span data-stu-id="af8c9-125">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="af8c9-126">Связи</span><span class="sxs-lookup"><span data-stu-id="af8c9-126">Relationships</span></span>

| <span data-ttu-id="af8c9-127">Связь</span><span class="sxs-lookup"><span data-stu-id="af8c9-127">Relationship</span></span> | <span data-ttu-id="af8c9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="af8c9-128">Type</span></span>        | <span data-ttu-id="af8c9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="af8c9-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af8c9-130">id</span><span class="sxs-lookup"><span data-stu-id="af8c9-130">id</span></span> |<span data-ttu-id="af8c9-131">String</span><span class="sxs-lookup"><span data-stu-id="af8c9-131">String</span></span>| <span data-ttu-id="af8c9-132">ИД объекта параметров для организации.</span><span class="sxs-lookup"><span data-stu-id="af8c9-132">Id of the settings object for the organization.</span></span> |
|<span data-ttu-id="af8c9-133">profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="af8c9-133">profileCardProperties</span></span>|<span data-ttu-id="af8c9-134">[Коллекция profileCardProperty](profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="af8c9-134">[profileCardProperty](profilecardproperty.md) collection</span></span>| <span data-ttu-id="af8c9-135">Содержит коллекцию свойств, которые администратор определил как видимые на карточке профиля Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="af8c9-135">Contains a collection of the properties an administrator has defined as visible on the Microsoft 365 profile card.</span></span> <span data-ttu-id="af8c9-136">[При этом возвращаются](../api/organizationsettings-get.md) свойства, настроенные для карт профилей организации.</span><span class="sxs-lookup"><span data-stu-id="af8c9-136">[Get organization settings](../api/organizationsettings-get.md) returns the properties configured for profile cards for the organization.</span></span>|
|<span data-ttu-id="af8c9-137">itemInsights</span><span class="sxs-lookup"><span data-stu-id="af8c9-137">itemInsights</span></span>|[<span data-ttu-id="af8c9-138">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="af8c9-138">itemInsightsSettings</span></span>](iteminsightssettings.md)| <span data-ttu-id="af8c9-139">Содержит свойства, настроенные администратором для видимости данных, полученных от Microsoft Graph, между пользователем и другими элементами в Microsoft 365, такими как документы или сайты.</span><span class="sxs-lookup"><span data-stu-id="af8c9-139">Contains the properties that are configured by an administrator for the visibility of Microsoft Graph-derived insights, between a user and other items in Microsoft 365, such as documents or sites.</span></span> <span data-ttu-id="af8c9-140">[Получите itemInsightsSettings через](../api/iteminsightssettings-get.md) это свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="af8c9-140">[Get itemInsightsSettings](../api/iteminsightssettings-get.md) through this navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af8c9-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af8c9-141">JSON representation</span></span>

<span data-ttu-id="af8c9-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af8c9-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


