---
title: тип ресурса параметров (eDiscovery)
description: Параметры для дела об обнаружении электронной почты
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 9f0248fa0c6080a143272d997b9d6125e0ccb5a2
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080881"
---
# <a name="settings-resource-type-ediscovery"></a><span data-ttu-id="4ac07-103">тип ресурса параметров (eDiscovery)</span><span class="sxs-lookup"><span data-stu-id="4ac07-103">settings resource type (eDiscovery)</span></span>

<span data-ttu-id="4ac07-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4ac07-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ac07-105">Параметры для дела об обнаружении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4ac07-105">Settings for an eDiscovery case.</span></span> <span data-ttu-id="4ac07-106">Подробные сведения [см. в материале Настройка параметров](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)поиска и аналитики в Advanced eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="4ac07-106">For details, see [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).</span></span>

<span data-ttu-id="4ac07-107">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="4ac07-107">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4ac07-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4ac07-108">Methods</span></span>

|<span data-ttu-id="4ac07-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4ac07-109">Method</span></span>|<span data-ttu-id="4ac07-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="4ac07-110">Return type</span></span>|<span data-ttu-id="4ac07-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ac07-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4ac07-112">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="4ac07-112">Get settings</span></span>](../api/ediscovery-settings-get.md)|[<span data-ttu-id="4ac07-113">microsoft.graph.ediscovery.settings</span><span class="sxs-lookup"><span data-stu-id="4ac07-113">microsoft.graph.ediscovery.settings</span></span>](../resources/ediscovery-settings.md)|<span data-ttu-id="4ac07-114">Ознакомьтесь с свойствами и отношениями объекта [microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="4ac07-114">Read the properties and relationships of a [microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md) object.</span></span>|
|[<span data-ttu-id="4ac07-115">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="4ac07-115">Update settings</span></span>](../api/ediscovery-settings-update.md)|[<span data-ttu-id="4ac07-116">microsoft.graph.ediscovery.settings</span><span class="sxs-lookup"><span data-stu-id="4ac07-116">microsoft.graph.ediscovery.settings</span></span>](../resources/ediscovery-settings.md)|<span data-ttu-id="4ac07-117">Обновление свойств объекта [microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="4ac07-117">Update the properties of a [microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md) object.</span></span>|
|[<span data-ttu-id="4ac07-118">resetToDefault</span><span class="sxs-lookup"><span data-stu-id="4ac07-118">resetToDefault</span></span>](../api/ediscovery-settings-resettodefault.md)|<span data-ttu-id="4ac07-119">Нет</span><span class="sxs-lookup"><span data-stu-id="4ac07-119">None</span></span>|<span data-ttu-id="4ac07-120">Сброс всех параметров в значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ac07-120">Reset all settings to the default values.</span></span>|

## <a name="properties"></a><span data-ttu-id="4ac07-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ac07-121">Properties</span></span>

|<span data-ttu-id="4ac07-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ac07-122">Property</span></span>|<span data-ttu-id="4ac07-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4ac07-123">Type</span></span>|<span data-ttu-id="4ac07-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4ac07-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ac07-125">Id</span><span class="sxs-lookup"><span data-stu-id="4ac07-125">Id</span></span>|<span data-ttu-id="4ac07-126">String</span><span class="sxs-lookup"><span data-stu-id="4ac07-126">String</span></span>|<span data-ttu-id="4ac07-127">ID дела об обнаружении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4ac07-127">The ID of the eDiscovery case.</span></span> <span data-ttu-id="4ac07-128">Наследуется от [сущности](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="4ac07-128">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="4ac07-129">ocr</span><span class="sxs-lookup"><span data-stu-id="4ac07-129">ocr</span></span>|[<span data-ttu-id="4ac07-130">microsoft.graph.ediscovery.ocrSettings</span><span class="sxs-lookup"><span data-stu-id="4ac07-130">microsoft.graph.ediscovery.ocrSettings</span></span>](../resources/ediscovery-ocrsettings.md)|<span data-ttu-id="4ac07-131">Параметры OCR (Optical Character Recognition) для дела.</span><span class="sxs-lookup"><span data-stu-id="4ac07-131">The OCR (Optical Character Recognition) settings for the case.</span></span>|
|<span data-ttu-id="4ac07-132">redundancyDetection</span><span class="sxs-lookup"><span data-stu-id="4ac07-132">redundancyDetection</span></span>|[<span data-ttu-id="4ac07-133">microsoft.graph.ediscovery.redundancyDetectionSettings</span><span class="sxs-lookup"><span data-stu-id="4ac07-133">microsoft.graph.ediscovery.redundancyDetectionSettings</span></span>](../resources/ediscovery-redundancydetectionsettings.md)|<span data-ttu-id="4ac07-134">Параметры обнаружения избыточности (рядом с дубликатом и потоком электронной почты) для дела.</span><span class="sxs-lookup"><span data-stu-id="4ac07-134">The redundancy (near duplicate and email threading) detection settings for the case.</span></span>|
|<span data-ttu-id="4ac07-135">topicModeling</span><span class="sxs-lookup"><span data-stu-id="4ac07-135">topicModeling</span></span>|[<span data-ttu-id="4ac07-136">microsoft.graph.ediscovery.topicModelingSettings</span><span class="sxs-lookup"><span data-stu-id="4ac07-136">microsoft.graph.ediscovery.topicModelingSettings</span></span>](../resources/ediscovery-topicmodelingsettings.md)|<span data-ttu-id="4ac07-137">Параметры моделирования тем (Темы) для дела.</span><span class="sxs-lookup"><span data-stu-id="4ac07-137">The Topic Modeling (Themes) settings for the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ac07-138">Связи</span><span class="sxs-lookup"><span data-stu-id="4ac07-138">Relationships</span></span>

<span data-ttu-id="4ac07-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4ac07-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ac07-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ac07-140">JSON representation</span></span>

<span data-ttu-id="4ac07-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ac07-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.settings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.settings",
  "id": "String (identifier)",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
  }
}
```
