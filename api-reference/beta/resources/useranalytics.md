---
title: Тип ресурса Усераналитикс
description: Параметры пользователя и статистика действий.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ac4024fff534bd89e369f1f8048ca274ccfd157a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057908"
---
# <a name="useranalytics-resource-type"></a><span data-ttu-id="4e5eb-103">Тип ресурса Усераналитикс</span><span class="sxs-lookup"><span data-stu-id="4e5eb-103">userAnalytics resource type</span></span>

<span data-ttu-id="4e5eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e5eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e5eb-105">Параметры пользователя и статистика действий.</span><span class="sxs-lookup"><span data-stu-id="4e5eb-105">The user's settings and activity statistics.</span></span>

## <a name="methods"></a><span data-ttu-id="4e5eb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4e5eb-106">Methods</span></span>

| <span data-ttu-id="4e5eb-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4e5eb-107">Method</span></span>       | <span data-ttu-id="4e5eb-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e5eb-108">Return Type</span></span> | <span data-ttu-id="4e5eb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e5eb-109">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="4e5eb-110">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="4e5eb-110">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="4e5eb-111">settings</span><span class="sxs-lookup"><span data-stu-id="4e5eb-111">settings</span></span>](settings.md) | <span data-ttu-id="4e5eb-112">Получение параметров пользователя для использования API аналитики.</span><span class="sxs-lookup"><span data-stu-id="4e5eb-112">Get the user's settings for using the analytics API.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e5eb-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e5eb-113">Properties</span></span>

| <span data-ttu-id="4e5eb-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e5eb-114">Property</span></span>     | <span data-ttu-id="4e5eb-115">Тип</span><span class="sxs-lookup"><span data-stu-id="4e5eb-115">Type</span></span>        | <span data-ttu-id="4e5eb-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4e5eb-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4e5eb-117">settings</span><span class="sxs-lookup"><span data-stu-id="4e5eb-117">settings</span></span>|[<span data-ttu-id="4e5eb-118">settings</span><span class="sxs-lookup"><span data-stu-id="4e5eb-118">settings</span></span>](settings.md)|<span data-ttu-id="4e5eb-119">Текущие параметры пользователя для использования API аналитики.</span><span class="sxs-lookup"><span data-stu-id="4e5eb-119">The current settings for a user to use the analytics API.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e5eb-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4e5eb-120">Relationships</span></span>

| <span data-ttu-id="4e5eb-121">Связь</span><span class="sxs-lookup"><span data-stu-id="4e5eb-121">Relationship</span></span> | <span data-ttu-id="4e5eb-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4e5eb-122">Type</span></span>        | <span data-ttu-id="4e5eb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4e5eb-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4e5eb-124">активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="4e5eb-124">activityStatistics</span></span>|<span data-ttu-id="4e5eb-125">Коллекция [активитистатистикс](activitystatistics.md)</span><span class="sxs-lookup"><span data-stu-id="4e5eb-125">[activityStatistics](activitystatistics.md) collection</span></span>| <span data-ttu-id="4e5eb-126">Коллекция рабочих действий, затраченных пользователем во время и за пределами рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="4e5eb-126">The collection of work activities that a user spent time on during and outside of working hours.</span></span> <span data-ttu-id="4e5eb-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e5eb-127">Read-only.</span></span> <span data-ttu-id="4e5eb-128">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4e5eb-128">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e5eb-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e5eb-129">JSON representation</span></span>

<span data-ttu-id="4e5eb-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e5eb-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "activityStatistics"
  ],
  "@odata.type": "microsoft.graph.userAnalytics"
}-->

```json
{
  "id": "string",
  "settings": {"@odata.type": "microsoft.graph.settings"},
  "activityStatistics": [{"@odata.type": "microsoft.graph.activityStatistics"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAnalytics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


