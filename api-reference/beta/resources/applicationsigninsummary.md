---
title: Тип ресурса applicationSignInDetailedSummary
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 454c4e2e9e57b61194e6f3e6970e5db1ea414369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137412"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="28d34-103">Тип ресурса applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="28d34-103">applicationSignInSummary resource type</span></span>

<span data-ttu-id="28d34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28d34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28d34-105">Представляет сводку по входу в приложение.</span><span class="sxs-lookup"><span data-stu-id="28d34-105">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="28d34-106">Методы</span><span class="sxs-lookup"><span data-stu-id="28d34-106">Methods</span></span>

| <span data-ttu-id="28d34-107">Метод</span><span class="sxs-lookup"><span data-stu-id="28d34-107">Method</span></span>       | <span data-ttu-id="28d34-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28d34-108">Return Type</span></span> | <span data-ttu-id="28d34-109">Описание</span><span class="sxs-lookup"><span data-stu-id="28d34-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="28d34-110">Получение applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="28d34-110">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="28d34-111">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="28d34-111">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="28d34-112">Чтение свойств и связей объекта **applicationSignInSummary.**</span><span class="sxs-lookup"><span data-stu-id="28d34-112">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="28d34-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="28d34-113">Properties</span></span>
| <span data-ttu-id="28d34-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="28d34-114">Property</span></span>     | <span data-ttu-id="28d34-115">Тип</span><span class="sxs-lookup"><span data-stu-id="28d34-115">Type</span></span>        | <span data-ttu-id="28d34-116">Описание</span><span class="sxs-lookup"><span data-stu-id="28d34-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28d34-117">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="28d34-117">appDisplayName</span></span>|<span data-ttu-id="28d34-118">String</span><span class="sxs-lookup"><span data-stu-id="28d34-118">String</span></span>|<span data-ttu-id="28d34-119">Имя приложения, в которое вписались пользователи.</span><span class="sxs-lookup"><span data-stu-id="28d34-119">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="28d34-120">appId</span><span class="sxs-lookup"><span data-stu-id="28d34-120">appId</span></span>|<span data-ttu-id="28d34-121">String</span><span class="sxs-lookup"><span data-stu-id="28d34-121">String</span></span>|  <span data-ttu-id="28d34-122">ИД приложения, подписанного пользователем i nto.</span><span class="sxs-lookup"><span data-stu-id="28d34-122">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="28d34-123">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="28d34-123">failedSignInCount</span></span>|<span data-ttu-id="28d34-124">Int64</span><span class="sxs-lookup"><span data-stu-id="28d34-124">Int64</span></span>|<span data-ttu-id="28d34-125">Количество неудачных входов в приложение.</span><span class="sxs-lookup"><span data-stu-id="28d34-125">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="28d34-126">successPercentage</span><span class="sxs-lookup"><span data-stu-id="28d34-126">successPercentage</span></span>|<span data-ttu-id="28d34-127">Int32</span><span class="sxs-lookup"><span data-stu-id="28d34-127">Int32</span></span>|<span data-ttu-id="28d34-128">Процент успешных входов, сделанных приложением.</span><span class="sxs-lookup"><span data-stu-id="28d34-128">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="28d34-129">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="28d34-129">successfulSignInCount</span></span>|<span data-ttu-id="28d34-130">Int64</span><span class="sxs-lookup"><span data-stu-id="28d34-130">Int64</span></span>|<span data-ttu-id="28d34-131">Количество успешных входов, сделанных приложением.</span><span class="sxs-lookup"><span data-stu-id="28d34-131">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28d34-132">Связи</span><span class="sxs-lookup"><span data-stu-id="28d34-132">Relationships</span></span>
<span data-ttu-id="28d34-133">Нет</span><span class="sxs-lookup"><span data-stu-id="28d34-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="28d34-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28d34-134">JSON representation</span></span>

<span data-ttu-id="28d34-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28d34-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInSummary"
}-->

```json
{
  "appDisplayName": "String",
  "appId": "String (identifier)",
  "failedSignInCount": 1024,
  "successPercentage": 1024,
  "successfulSignInCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


