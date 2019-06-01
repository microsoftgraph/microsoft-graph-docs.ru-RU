---
title: Тип ресурса Аппликатионсигниндетаиледсуммари
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c6ecd91bb29abc409a745e92b523948b78552ed4
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657625"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="55ee3-103">Тип ресурса Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="55ee3-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55ee3-104">Представляет сводку по входу в приложение.</span><span class="sxs-lookup"><span data-stu-id="55ee3-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="55ee3-105">Методы</span><span class="sxs-lookup"><span data-stu-id="55ee3-105">Methods</span></span>

| <span data-ttu-id="55ee3-106">Метод</span><span class="sxs-lookup"><span data-stu-id="55ee3-106">Method</span></span>       | <span data-ttu-id="55ee3-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55ee3-107">Return Type</span></span> | <span data-ttu-id="55ee3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="55ee3-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="55ee3-109">Получение Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="55ee3-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="55ee3-110">Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="55ee3-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="55ee3-111">Чтение свойств и связей объекта **аппликатионсигнинсуммари** .</span><span class="sxs-lookup"><span data-stu-id="55ee3-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="55ee3-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="55ee3-112">Properties</span></span>
| <span data-ttu-id="55ee3-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="55ee3-113">Property</span></span>     | <span data-ttu-id="55ee3-114">Тип</span><span class="sxs-lookup"><span data-stu-id="55ee3-114">Type</span></span>        | <span data-ttu-id="55ee3-115">Описание</span><span class="sxs-lookup"><span data-stu-id="55ee3-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="55ee3-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="55ee3-116">appDisplayName</span></span>|<span data-ttu-id="55ee3-117">String</span><span class="sxs-lookup"><span data-stu-id="55ee3-117">String</span></span>|<span data-ttu-id="55ee3-118">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="55ee3-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="55ee3-119">appId</span><span class="sxs-lookup"><span data-stu-id="55ee3-119">appId</span></span>|<span data-ttu-id="55ee3-120">String</span><span class="sxs-lookup"><span data-stu-id="55ee3-120">String</span></span>|  <span data-ttu-id="55ee3-121">Идентификатор приложения, выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ee3-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="55ee3-122">Фаиледсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="55ee3-122">failedSignInCount</span></span>|<span data-ttu-id="55ee3-123">Int64</span><span class="sxs-lookup"><span data-stu-id="55ee3-123">Int64</span></span>|<span data-ttu-id="55ee3-124">Количество неудачных операций входа, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="55ee3-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="55ee3-125">Сукцессперцентаже</span><span class="sxs-lookup"><span data-stu-id="55ee3-125">successPercentage</span></span>|<span data-ttu-id="55ee3-126">Int32</span><span class="sxs-lookup"><span data-stu-id="55ee3-126">Int32</span></span>|<span data-ttu-id="55ee3-127">Процент успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="55ee3-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="55ee3-128">Сукцессфулсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="55ee3-128">successfulSignInCount</span></span>|<span data-ttu-id="55ee3-129">Int64</span><span class="sxs-lookup"><span data-stu-id="55ee3-129">Int64</span></span>|<span data-ttu-id="55ee3-130">Количество успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="55ee3-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55ee3-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="55ee3-131">Relationships</span></span>
<span data-ttu-id="55ee3-132">Нет</span><span class="sxs-lookup"><span data-stu-id="55ee3-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="55ee3-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55ee3-133">JSON representation</span></span>

<span data-ttu-id="55ee3-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55ee3-134">The following is a JSON representation of the resource.</span></span>

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
