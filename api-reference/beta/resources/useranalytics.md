---
title: Тип ресурса Усераналитикс
description: Параметры пользователя и статистика действий.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 51e72d21cfb0e26e46a7d247f4ede59b112893ea
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450801"
---
# <a name="useranalytics-resource-type"></a><span data-ttu-id="86039-103">Тип ресурса Усераналитикс</span><span class="sxs-lookup"><span data-stu-id="86039-103">userAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86039-104">Параметры пользователя и статистика действий.</span><span class="sxs-lookup"><span data-stu-id="86039-104">The user's settings and activity statistics.</span></span>

## <a name="methods"></a><span data-ttu-id="86039-105">Методы</span><span class="sxs-lookup"><span data-stu-id="86039-105">Methods</span></span>

| <span data-ttu-id="86039-106">Метод</span><span class="sxs-lookup"><span data-stu-id="86039-106">Method</span></span>       | <span data-ttu-id="86039-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="86039-107">Return Type</span></span> | <span data-ttu-id="86039-108">Описание</span><span class="sxs-lookup"><span data-stu-id="86039-108">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="86039-109">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="86039-109">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="86039-110">settings</span><span class="sxs-lookup"><span data-stu-id="86039-110">settings</span></span>](settings.md) | <span data-ttu-id="86039-111">Получение параметров пользователя для использования API аналитики.</span><span class="sxs-lookup"><span data-stu-id="86039-111">Get the user's settings for using the analytics API.</span></span>|

## <a name="properties"></a><span data-ttu-id="86039-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="86039-112">Properties</span></span>

| <span data-ttu-id="86039-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="86039-113">Property</span></span>     | <span data-ttu-id="86039-114">Тип</span><span class="sxs-lookup"><span data-stu-id="86039-114">Type</span></span>        | <span data-ttu-id="86039-115">Описание</span><span class="sxs-lookup"><span data-stu-id="86039-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86039-116">settings</span><span class="sxs-lookup"><span data-stu-id="86039-116">settings</span></span>|[<span data-ttu-id="86039-117">settings</span><span class="sxs-lookup"><span data-stu-id="86039-117">settings</span></span>](settings.md)|<span data-ttu-id="86039-118">Текущие параметры пользователя для использования API аналитики.</span><span class="sxs-lookup"><span data-stu-id="86039-118">The current settings for a user to use the analytics API.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86039-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="86039-119">Relationships</span></span>

| <span data-ttu-id="86039-120">Отношение</span><span class="sxs-lookup"><span data-stu-id="86039-120">Relationship</span></span> | <span data-ttu-id="86039-121">Тип</span><span class="sxs-lookup"><span data-stu-id="86039-121">Type</span></span>        | <span data-ttu-id="86039-122">Описание</span><span class="sxs-lookup"><span data-stu-id="86039-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86039-123">активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="86039-123">activityStatistics</span></span>|<span data-ttu-id="86039-124">Коллекция [активитистатистикс](activitystatistics.md)</span><span class="sxs-lookup"><span data-stu-id="86039-124">[activityStatistics](activitystatistics.md) collection</span></span>| <span data-ttu-id="86039-125">Коллекция рабочих действий, затраченных пользователем во время и за пределами рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="86039-125">The collection of work activities that a user spent time on during and outside of working hours.</span></span> <span data-ttu-id="86039-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86039-126">Read-only.</span></span> <span data-ttu-id="86039-127">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="86039-127">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86039-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86039-128">JSON representation</span></span>

<span data-ttu-id="86039-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86039-129">The following is a JSON representation of the resource.</span></span>

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
