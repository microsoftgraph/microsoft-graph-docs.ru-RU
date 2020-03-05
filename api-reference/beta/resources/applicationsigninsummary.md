---
title: Тип ресурса Аппликатионсигниндетаиледсуммари
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType_
ms.openlocfilehash: ed491c9bce61bdc7f9ae3821360832dd8cbe04e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508270"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="e1035-103">Тип ресурса Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="e1035-103">applicationSignInSummary resource type</span></span>

<span data-ttu-id="e1035-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e1035-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1035-105">Представляет сводку по входу в приложение.</span><span class="sxs-lookup"><span data-stu-id="e1035-105">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="e1035-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e1035-106">Methods</span></span>

| <span data-ttu-id="e1035-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e1035-107">Method</span></span>       | <span data-ttu-id="e1035-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e1035-108">Return Type</span></span> | <span data-ttu-id="e1035-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e1035-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e1035-110">Получение Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="e1035-110">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="e1035-111">аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="e1035-111">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="e1035-112">Чтение свойств и связей объекта **аппликатионсигнинсуммари** .</span><span class="sxs-lookup"><span data-stu-id="e1035-112">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e1035-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1035-113">Properties</span></span>
| <span data-ttu-id="e1035-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1035-114">Property</span></span>     | <span data-ttu-id="e1035-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e1035-115">Type</span></span>        | <span data-ttu-id="e1035-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e1035-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1035-117">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="e1035-117">appDisplayName</span></span>|<span data-ttu-id="e1035-118">String</span><span class="sxs-lookup"><span data-stu-id="e1035-118">String</span></span>|<span data-ttu-id="e1035-119">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="e1035-119">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="e1035-120">appId</span><span class="sxs-lookup"><span data-stu-id="e1035-120">appId</span></span>|<span data-ttu-id="e1035-121">String</span><span class="sxs-lookup"><span data-stu-id="e1035-121">String</span></span>|  <span data-ttu-id="e1035-122">Идентификатор приложения, выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1035-122">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="e1035-123">фаиледсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="e1035-123">failedSignInCount</span></span>|<span data-ttu-id="e1035-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e1035-124">Int64</span></span>|<span data-ttu-id="e1035-125">Количество неудачных операций входа, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="e1035-125">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="e1035-126">сукцессперцентаже</span><span class="sxs-lookup"><span data-stu-id="e1035-126">successPercentage</span></span>|<span data-ttu-id="e1035-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e1035-127">Int32</span></span>|<span data-ttu-id="e1035-128">Процент успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="e1035-128">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="e1035-129">сукцессфулсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="e1035-129">successfulSignInCount</span></span>|<span data-ttu-id="e1035-130">Int64</span><span class="sxs-lookup"><span data-stu-id="e1035-130">Int64</span></span>|<span data-ttu-id="e1035-131">Количество успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="e1035-131">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1035-132">Связи</span><span class="sxs-lookup"><span data-stu-id="e1035-132">Relationships</span></span>
<span data-ttu-id="e1035-133">Нет</span><span class="sxs-lookup"><span data-stu-id="e1035-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e1035-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1035-134">JSON representation</span></span>

<span data-ttu-id="e1035-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1035-135">The following is a JSON representation of the resource.</span></span>

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
