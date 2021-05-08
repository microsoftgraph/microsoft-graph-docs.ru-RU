---
title: accessReviewHistoryDefinition resource types
description: Представляет коллекцию данных истории обзоров доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 96619cb95c11a77106c86cbdcc720f1a486721c7
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232977"
---
# <a name="accessreviewhistorydefinition-resource-type"></a><span data-ttu-id="3753c-103">тип ресурса accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="3753c-103">accessReviewHistoryDefinition resource type</span></span>

<span data-ttu-id="3753c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3753c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3753c-105">Представляет коллекцию данных истории обзоров доступа и области, используемые для сбора этих данных.</span><span class="sxs-lookup"><span data-stu-id="3753c-105">Represents a collection of access review history data and the scopes used to collect that data.</span></span> <span data-ttu-id="3753c-106">**ReviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime** **,**  решения и области свойств **accessReviewHistoryDefinition** используются при выборе данных истории отзывов и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3753c-106">The **reviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime**, **decisions**, and **scopes** properties of an **accessReviewHistoryDefinition** are used when selecting review history data, and can be modified.</span></span> <span data-ttu-id="3753c-107">Каждый **объект accessReviewHistoryDefinition** доступен только в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="3753c-107">Each **accessReviewHistoryDefinition** object is only available for 30 days.</span></span> <span data-ttu-id="3753c-108">После того, как состояние определения истории переместилось на ссылку, можно создать для получения данных определения с помощью вызова `done` [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md).</span><span class="sxs-lookup"><span data-stu-id="3753c-108">Once a history definition's status has moved to `done` a link can be generated to retrieve the definition's data by calling [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3753c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3753c-109">Methods</span></span>
|<span data-ttu-id="3753c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3753c-110">Method</span></span>|<span data-ttu-id="3753c-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="3753c-111">Return type</span></span>|<span data-ttu-id="3753c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3753c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3753c-113">Список accessReviewHistoryDefinitions</span><span class="sxs-lookup"><span data-stu-id="3753c-113">List accessReviewHistoryDefinitions</span></span>](../api/accessreviewhistorydefinition-list.md)|<span data-ttu-id="3753c-114">[accessReviewHistoryDefinition collection](accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3753c-114">[accessReviewHistoryDefinition](accessreviewhistorydefinition.md) collection</span></span>|<span data-ttu-id="3753c-115">Получите список объектов [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="3753c-115">Get a list of the [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) objects and their properties.</span></span>|
|[<span data-ttu-id="3753c-116">Создание accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="3753c-116">Create accessReviewHistoryDefinition</span></span>](../api/accessreviewhistorydefinition-post.md)|[<span data-ttu-id="3753c-117">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="3753c-117">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="3753c-118">Создайте новый [объект accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3753c-118">Create a new [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) object.</span></span>|
|[<span data-ttu-id="3753c-119">Получить accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="3753c-119">Get accessReviewHistoryDefinition</span></span>](../api/accessreviewhistorydefinition-get.md)|[<span data-ttu-id="3753c-120">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="3753c-120">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="3753c-121">Ознакомьтесь с свойствами и отношениями [объекта accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3753c-121">Read the properties and relationships of an [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) object.</span></span>|
|[<span data-ttu-id="3753c-122">generateDownloadUri</span><span class="sxs-lookup"><span data-stu-id="3753c-122">generateDownloadUri</span></span>](../api/accessreviewhistorydefinition-generatedownloaduri.md)|[<span data-ttu-id="3753c-123">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="3753c-123">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="3753c-124">Создание URI, который можно использовать для получения данных истории отзывов.</span><span class="sxs-lookup"><span data-stu-id="3753c-124">Generate a URI that can be used to retrieve review history data.</span></span>|

## <a name="properties"></a><span data-ttu-id="3753c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="3753c-125">Properties</span></span>
|<span data-ttu-id="3753c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3753c-126">Property</span></span>|<span data-ttu-id="3753c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3753c-127">Type</span></span>|<span data-ttu-id="3753c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3753c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3753c-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="3753c-129">createdBy</span></span>|[<span data-ttu-id="3753c-130">userIdentity</span><span class="sxs-lookup"><span data-stu-id="3753c-130">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="3753c-131">Пользователь, создавший это определение истории обзора.</span><span class="sxs-lookup"><span data-stu-id="3753c-131">User who created this review history definition.</span></span> |
|<span data-ttu-id="3753c-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3753c-132">createdDateTime</span></span>|<span data-ttu-id="3753c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3753c-133">DateTimeOffset</span></span>|<span data-ttu-id="3753c-134">Timestamp, когда было создано определение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="3753c-134">Timestamp when the access review definition was created.</span></span>|
|<span data-ttu-id="3753c-135">решения</span><span class="sxs-lookup"><span data-stu-id="3753c-135">decisions</span></span>|<span data-ttu-id="3753c-136">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3753c-136">String collection</span></span>|<span data-ttu-id="3753c-137">Определяет, какие решения по проверке будут включены в данные истории проверки, если заданы.</span><span class="sxs-lookup"><span data-stu-id="3753c-137">Determines which review decisions will be included in the fetched review history data if specified.</span></span> <span data-ttu-id="3753c-138">Необязательный для создания.</span><span class="sxs-lookup"><span data-stu-id="3753c-138">Optional on create.</span></span> <span data-ttu-id="3753c-139">Все решения будут включены по умолчанию, если не будут предоставлены решения о создании.</span><span class="sxs-lookup"><span data-stu-id="3753c-139">All decisions will be included by default if no decisions are provided on create.</span></span> <span data-ttu-id="3753c-140">Возможные значения: `approve` `deny` , , , , `dontKnow` и `notReviewed` `notNotified` .</span><span class="sxs-lookup"><span data-stu-id="3753c-140">Possible values are: `approve`, `deny`, `dontKnow`, `notReviewed`, and `notNotified`.</span></span>|
|<span data-ttu-id="3753c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="3753c-141">displayName</span></span>|<span data-ttu-id="3753c-142">String</span><span class="sxs-lookup"><span data-stu-id="3753c-142">String</span></span>|<span data-ttu-id="3753c-143">Имя для сбора данных истории проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="3753c-143">Name for the access review history data collection.</span></span> <span data-ttu-id="3753c-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3753c-144">Required.</span></span>|
|<span data-ttu-id="3753c-145">downloadUri</span><span class="sxs-lookup"><span data-stu-id="3753c-145">downloadUri</span></span>|<span data-ttu-id="3753c-146">String</span><span class="sxs-lookup"><span data-stu-id="3753c-146">String</span></span>|<span data-ttu-id="3753c-147">Uri, которые можно использовать для получения данных истории отзывов.</span><span class="sxs-lookup"><span data-stu-id="3753c-147">Uri which can be used to retrieve review history data.</span></span> <span data-ttu-id="3753c-148">Этот URI будет активен в течение 24 часов после сгенерирований.</span><span class="sxs-lookup"><span data-stu-id="3753c-148">This URI will be active for 24 hours after being generated.</span></span>|
|<span data-ttu-id="3753c-149">fulfilledDateTime</span><span class="sxs-lookup"><span data-stu-id="3753c-149">fulfilledDateTime</span></span>|<span data-ttu-id="3753c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3753c-150">DateTimeOffset</span></span>|<span data-ttu-id="3753c-151">Timestamp, когда все доступные данные для этого определения были собраны.</span><span class="sxs-lookup"><span data-stu-id="3753c-151">Timestamp when all of the available data for this definition was collected.</span></span> <span data-ttu-id="3753c-152">Это будет установлено после того, как будет заданной для этого определения состояние `done` .</span><span class="sxs-lookup"><span data-stu-id="3753c-152">This will be set after this definition's status is set to `done`.</span></span>|
|<span data-ttu-id="3753c-153">id</span><span class="sxs-lookup"><span data-stu-id="3753c-153">id</span></span>|<span data-ttu-id="3753c-154">String</span><span class="sxs-lookup"><span data-stu-id="3753c-154">String</span></span>|<span data-ttu-id="3753c-155">Назначен уникальный идентификатор определения истории проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="3753c-155">The assigned unique identifier of an access review history definition.</span></span>|
|<span data-ttu-id="3753c-156">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="3753c-156">reviewHistoryPeriodEndDateTime</span></span>|<span data-ttu-id="3753c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3753c-157">DateTimeOffset</span></span>|<span data-ttu-id="3753c-158">Timestamp, отзывы, начиная с этой даты или после нее, будут включены в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="3753c-158">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="3753c-159">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3753c-159">Required.</span></span>|
|<span data-ttu-id="3753c-160">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="3753c-160">reviewHistoryPeriodStartDateTime</span></span>|<span data-ttu-id="3753c-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3753c-161">DateTimeOffset</span></span>|<span data-ttu-id="3753c-162">Timestamp, отзывы, начиная с этой даты или до этой даты, будут включены в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="3753c-162">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="3753c-163">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3753c-163">Required.</span></span>|
|<span data-ttu-id="3753c-164">scopes</span><span class="sxs-lookup"><span data-stu-id="3753c-164">scopes</span></span>|<span data-ttu-id="3753c-165">коллекция microsoft.graph.accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="3753c-165">microsoft.graph.accessReviewQueryScope collection</span></span>|<span data-ttu-id="3753c-166">Используется для области, включаемой отзывов в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="3753c-166">Used to scope what reviews are included in the fetched history data.</span></span> <span data-ttu-id="3753c-167">Извлекает отзывы, область которых совпадает с этой предоставленной областью.</span><span class="sxs-lookup"><span data-stu-id="3753c-167">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="3753c-168">См. [accessreviewqueryscope](accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="3753c-168">See [accessreviewqueryscope](accessreviewqueryscope.md).</span></span> <span data-ttu-id="3753c-169">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3753c-169">Required.</span></span>|
|<span data-ttu-id="3753c-170">status</span><span class="sxs-lookup"><span data-stu-id="3753c-170">status</span></span>|<span data-ttu-id="3753c-171">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3753c-171">String collection</span></span>|<span data-ttu-id="3753c-172">Представляет состояние коллекции данных истории отзывов.</span><span class="sxs-lookup"><span data-stu-id="3753c-172">Represents the status of the review history data collection.</span></span> <span data-ttu-id="3753c-173">Возможные значения: `done`, `inprogress`, `error`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="3753c-173">Possible values are: `done`, `inprogress`, `error`, `requested`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3753c-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3753c-174">JSON representation</span></span>
<span data-ttu-id="3753c-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3753c-175">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "decisions": [
    {
      "@odata.type": "String"
    }
  ],
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "createdBy": {
    "@odata.type": "#microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    }
  ]
}
```
