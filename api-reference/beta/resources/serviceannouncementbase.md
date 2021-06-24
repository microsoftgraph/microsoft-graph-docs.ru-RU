---
title: тип ресурса serviceAnnouncementBase
description: Это абстрактный базовый тип для serviceHealthIssue и serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 46e1e6428d1371683a8ad1febae990146a9fe898
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109241"
---
# <a name="serviceannouncementbase-resource-type"></a><span data-ttu-id="9e269-103">тип ресурса serviceAnnouncementBase</span><span class="sxs-lookup"><span data-stu-id="9e269-103">serviceAnnouncementBase resource type</span></span>

<span data-ttu-id="9e269-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e269-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e269-105">Это абстрактный базовый тип [для serviceHealthIssue](../resources/servicehealthissue.md) и [serviceUpdateMessage.](../resources/serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="9e269-105">This is an abstract base type for [serviceHealthIssue](../resources/servicehealthissue.md) and [serviceUpdateMessage](../resources/serviceupdatemessage.md).</span></span>

<span data-ttu-id="9e269-106">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="9e269-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9e269-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9e269-107">Methods</span></span>
<span data-ttu-id="9e269-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e269-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="9e269-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e269-109">Properties</span></span>
|<span data-ttu-id="9e269-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e269-110">Property</span></span>|<span data-ttu-id="9e269-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9e269-111">Type</span></span>|<span data-ttu-id="9e269-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9e269-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e269-113">подробности</span><span class="sxs-lookup"><span data-stu-id="9e269-113">details</span></span>|<span data-ttu-id="9e269-114">[Коллекция(keyValuePair)](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9e269-114">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="9e269-115">Дополнительные сведения о событии службы.</span><span class="sxs-lookup"><span data-stu-id="9e269-115">Additional details about service event.</span></span> <span data-ttu-id="9e269-116">Это свойство не поддерживает фильтры.</span><span class="sxs-lookup"><span data-stu-id="9e269-116">This property doesn't support filters.</span></span>|
|<span data-ttu-id="9e269-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9e269-117">endDateTime</span></span>|<span data-ttu-id="9e269-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e269-118">DateTimeOffset</span></span>|<span data-ttu-id="9e269-119">Конечное время события службы.</span><span class="sxs-lookup"><span data-stu-id="9e269-119">The end time of the service event.</span></span>|
|<span data-ttu-id="9e269-120">id</span><span class="sxs-lookup"><span data-stu-id="9e269-120">id</span></span>|<span data-ttu-id="9e269-121">Строка</span><span class="sxs-lookup"><span data-stu-id="9e269-121">String</span></span>|<span data-ttu-id="9e269-122">Id события службы.</span><span class="sxs-lookup"><span data-stu-id="9e269-122">The id of the service event.</span></span>|
|<span data-ttu-id="9e269-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e269-123">lastModifiedDateTime</span></span>|<span data-ttu-id="9e269-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e269-124">DateTimeOffset</span></span>|<span data-ttu-id="9e269-125">Последнее измененное время события службы.</span><span class="sxs-lookup"><span data-stu-id="9e269-125">The last modified time of the service event.</span></span>|
|<span data-ttu-id="9e269-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e269-126">startDateTime</span></span>|<span data-ttu-id="9e269-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e269-127">DateTimeOffset</span></span>|<span data-ttu-id="9e269-128">Время начала события службы.</span><span class="sxs-lookup"><span data-stu-id="9e269-128">The start time of the service event.</span></span>|
|<span data-ttu-id="9e269-129">title</span><span class="sxs-lookup"><span data-stu-id="9e269-129">title</span></span>|<span data-ttu-id="9e269-130">Строка</span><span class="sxs-lookup"><span data-stu-id="9e269-130">String</span></span>|<span data-ttu-id="9e269-131">Название события службы.</span><span class="sxs-lookup"><span data-stu-id="9e269-131">The title of the service event.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e269-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="9e269-132">Relationships</span></span>
<span data-ttu-id="9e269-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e269-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e269-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9e269-134">JSON representation</span></span>
<span data-ttu-id="9e269-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e269-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementBase",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```