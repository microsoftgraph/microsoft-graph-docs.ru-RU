---
title: тип ресурса serviceAnnouncement
description: Контейнер верхнего уровня для ресурсов связи службы
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c22cbcd9fd8e67137e649cc099ff7980468c246f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109244"
---
# <a name="serviceannouncement-resource-type"></a><span data-ttu-id="27cd0-103">тип ресурса serviceAnnouncement</span><span class="sxs-lookup"><span data-stu-id="27cd0-103">serviceAnnouncement resource type</span></span>

<span data-ttu-id="27cd0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27cd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27cd0-105">Контейнер верхнего уровня для ресурсов связи службы.</span><span class="sxs-lookup"><span data-stu-id="27cd0-105">A top-level container for service communications resources.</span></span>

## <a name="methods"></a><span data-ttu-id="27cd0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="27cd0-106">Methods</span></span>
|<span data-ttu-id="27cd0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="27cd0-107">Method</span></span>|<span data-ttu-id="27cd0-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="27cd0-108">Return type</span></span>|<span data-ttu-id="27cd0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="27cd0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27cd0-110">Список healthOverviews</span><span class="sxs-lookup"><span data-stu-id="27cd0-110">List healthOverviews</span></span>](../api/serviceannouncement-list-healthoverviews.md)|<span data-ttu-id="27cd0-111">[коллекция serviceHealth](../resources/servicehealth.md)</span><span class="sxs-lookup"><span data-stu-id="27cd0-111">[serviceHealth](../resources/servicehealth.md) collection</span></span>|<span data-ttu-id="27cd0-112">Получите ресурсы serviceHealth из свойства навигации healthOverviews.</span><span class="sxs-lookup"><span data-stu-id="27cd0-112">Get the serviceHealth resources from the healthOverviews navigation property.</span></span>|
|[<span data-ttu-id="27cd0-113">Проблемы со списком</span><span class="sxs-lookup"><span data-stu-id="27cd0-113">List issues</span></span>](../api/serviceannouncement-list-issues.md)|<span data-ttu-id="27cd0-114">[коллекция serviceHealthIssue](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="27cd0-114">[serviceHealthIssue](../resources/servicehealthissue.md) collection</span></span>|<span data-ttu-id="27cd0-115">Получите ресурсы serviceHealthIssue из свойства навигации проблем.</span><span class="sxs-lookup"><span data-stu-id="27cd0-115">Get the serviceHealthIssue resources from the issues navigation property.</span></span>|
|[<span data-ttu-id="27cd0-116">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="27cd0-116">List messages</span></span>](../api/serviceannouncement-list-messages.md)|<span data-ttu-id="27cd0-117">[коллекция serviceUpdateMessage](../resources/serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="27cd0-117">[serviceUpdateMessage](../resources/serviceupdatemessage.md) collection</span></span>|<span data-ttu-id="27cd0-118">Получите ресурсы serviceUpdateMessage из свойства навигации сообщений.</span><span class="sxs-lookup"><span data-stu-id="27cd0-118">Get the serviceUpdateMessage resources from the messages navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="27cd0-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="27cd0-119">Properties</span></span>
<span data-ttu-id="27cd0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="27cd0-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="27cd0-121">Связи</span><span class="sxs-lookup"><span data-stu-id="27cd0-121">Relationships</span></span>
|<span data-ttu-id="27cd0-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="27cd0-122">Property</span></span>|<span data-ttu-id="27cd0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="27cd0-123">Type</span></span>|<span data-ttu-id="27cd0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="27cd0-124">Description</span></span>|
|-|-|-|
|<span data-ttu-id="27cd0-125">messages</span><span class="sxs-lookup"><span data-stu-id="27cd0-125">messages</span></span>|<span data-ttu-id="27cd0-126">[Collection(serviceUpdateMessage)](serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="27cd0-126">Collection([serviceUpdateMessage](serviceupdatemessage.md))</span></span>|<span data-ttu-id="27cd0-127">Коллекция сообщений службы для клиента.</span><span class="sxs-lookup"><span data-stu-id="27cd0-127">A collection of service messages for tenant.</span></span> <span data-ttu-id="27cd0-128">Это свойство содержит свойство навигации, оно является недействительным и читаемым.</span><span class="sxs-lookup"><span data-stu-id="27cd0-128">This property is a contained navigation property, it is nullable and readonly.</span></span>|
|<span data-ttu-id="27cd0-129">healthOverviews</span><span class="sxs-lookup"><span data-stu-id="27cd0-129">healthOverviews</span></span>|<span data-ttu-id="27cd0-130">[Collection(serviceHealth)](servicehealth.md)</span><span class="sxs-lookup"><span data-stu-id="27cd0-130">Collection([serviceHealth](servicehealth.md))</span></span>|<span data-ttu-id="27cd0-131">Коллекция сведений о состоянии здоровья служб для клиента.</span><span class="sxs-lookup"><span data-stu-id="27cd0-131">A collection of service health information for tenant.</span></span> <span data-ttu-id="27cd0-132">Это свойство содержит свойство навигации, оно является недействительным и читаемым.</span><span class="sxs-lookup"><span data-stu-id="27cd0-132">This property is a contained navigation property, it is nullable and readonly.</span></span>|
|<span data-ttu-id="27cd0-133">проблемы</span><span class="sxs-lookup"><span data-stu-id="27cd0-133">issues</span></span>|<span data-ttu-id="27cd0-134">[Collection(serviceHealthIssue)](servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="27cd0-134">Collection([serviceHealthIssue](servicehealthissue.md))</span></span>|<span data-ttu-id="27cd0-135">Набор проблем с обслуживанием для клиента.</span><span class="sxs-lookup"><span data-stu-id="27cd0-135">A collection of service issues for tenant.</span></span> <span data-ttu-id="27cd0-136">Это свойство содержит свойство навигации, оно является недействительным и читаемым.</span><span class="sxs-lookup"><span data-stu-id="27cd0-136">This property is a contained navigation property, it is nullable and readonly.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27cd0-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27cd0-137">JSON representation</span></span>
<span data-ttu-id="27cd0-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27cd0-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncement"
}
```