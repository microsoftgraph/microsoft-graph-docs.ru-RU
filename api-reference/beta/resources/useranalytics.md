---
title: Тип ресурса Усераналитикс
description: Параметры пользователя и статистика действий.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ffe6830088bd60c4de9cea8def8e8202d1b33f13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519542"
---
# <a name="useranalytics-resource-type"></a><span data-ttu-id="63960-103">Тип ресурса Усераналитикс</span><span class="sxs-lookup"><span data-stu-id="63960-103">userAnalytics resource type</span></span>

<span data-ttu-id="63960-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="63960-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63960-105">Параметры пользователя и статистика действий.</span><span class="sxs-lookup"><span data-stu-id="63960-105">The user's settings and activity statistics.</span></span>

## <a name="methods"></a><span data-ttu-id="63960-106">Методы</span><span class="sxs-lookup"><span data-stu-id="63960-106">Methods</span></span>

| <span data-ttu-id="63960-107">Метод</span><span class="sxs-lookup"><span data-stu-id="63960-107">Method</span></span>       | <span data-ttu-id="63960-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="63960-108">Return Type</span></span> | <span data-ttu-id="63960-109">Описание</span><span class="sxs-lookup"><span data-stu-id="63960-109">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="63960-110">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="63960-110">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="63960-111">settings</span><span class="sxs-lookup"><span data-stu-id="63960-111">settings</span></span>](settings.md) | <span data-ttu-id="63960-112">Получение параметров пользователя для использования API аналитики.</span><span class="sxs-lookup"><span data-stu-id="63960-112">Get the user's settings for using the analytics API.</span></span>|

## <a name="properties"></a><span data-ttu-id="63960-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="63960-113">Properties</span></span>

| <span data-ttu-id="63960-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="63960-114">Property</span></span>     | <span data-ttu-id="63960-115">Тип</span><span class="sxs-lookup"><span data-stu-id="63960-115">Type</span></span>        | <span data-ttu-id="63960-116">Описание</span><span class="sxs-lookup"><span data-stu-id="63960-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63960-117">settings</span><span class="sxs-lookup"><span data-stu-id="63960-117">settings</span></span>|[<span data-ttu-id="63960-118">settings</span><span class="sxs-lookup"><span data-stu-id="63960-118">settings</span></span>](settings.md)|<span data-ttu-id="63960-119">Текущие параметры пользователя для использования API аналитики.</span><span class="sxs-lookup"><span data-stu-id="63960-119">The current settings for a user to use the analytics API.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63960-120">Связи</span><span class="sxs-lookup"><span data-stu-id="63960-120">Relationships</span></span>

| <span data-ttu-id="63960-121">Связь</span><span class="sxs-lookup"><span data-stu-id="63960-121">Relationship</span></span> | <span data-ttu-id="63960-122">Тип</span><span class="sxs-lookup"><span data-stu-id="63960-122">Type</span></span>        | <span data-ttu-id="63960-123">Описание</span><span class="sxs-lookup"><span data-stu-id="63960-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63960-124">активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="63960-124">activityStatistics</span></span>|<span data-ttu-id="63960-125">Коллекция [активитистатистикс](activitystatistics.md)</span><span class="sxs-lookup"><span data-stu-id="63960-125">[activityStatistics](activitystatistics.md) collection</span></span>| <span data-ttu-id="63960-126">Коллекция рабочих действий, затраченных пользователем во время и за пределами рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="63960-126">The collection of work activities that a user spent time on during and outside of working hours.</span></span> <span data-ttu-id="63960-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="63960-127">Read-only.</span></span> <span data-ttu-id="63960-128">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="63960-128">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63960-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63960-129">JSON representation</span></span>

<span data-ttu-id="63960-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63960-130">The following is a JSON representation of the resource.</span></span>

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
