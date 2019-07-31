---
title: Тип ресурса Аппликатионсигниндетаиледсуммари
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType_
ms.openlocfilehash: d169755679cd60285808c1c93cb31810b1d1939d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013341"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="6e017-103">Тип ресурса Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="6e017-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e017-104">Представляет сводку по входу в приложение.</span><span class="sxs-lookup"><span data-stu-id="6e017-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="6e017-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6e017-105">Methods</span></span>

| <span data-ttu-id="6e017-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6e017-106">Method</span></span>       | <span data-ttu-id="6e017-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6e017-107">Return Type</span></span> | <span data-ttu-id="6e017-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6e017-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6e017-109">Получение Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="6e017-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="6e017-110">Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="6e017-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="6e017-111">Чтение свойств и связей объекта **аппликатионсигнинсуммари** .</span><span class="sxs-lookup"><span data-stu-id="6e017-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6e017-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e017-112">Properties</span></span>
| <span data-ttu-id="6e017-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e017-113">Property</span></span>     | <span data-ttu-id="6e017-114">Тип</span><span class="sxs-lookup"><span data-stu-id="6e017-114">Type</span></span>        | <span data-ttu-id="6e017-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6e017-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e017-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="6e017-116">appDisplayName</span></span>|<span data-ttu-id="6e017-117">String</span><span class="sxs-lookup"><span data-stu-id="6e017-117">String</span></span>|<span data-ttu-id="6e017-118">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="6e017-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="6e017-119">appId</span><span class="sxs-lookup"><span data-stu-id="6e017-119">appId</span></span>|<span data-ttu-id="6e017-120">String</span><span class="sxs-lookup"><span data-stu-id="6e017-120">String</span></span>|  <span data-ttu-id="6e017-121">Идентификатор приложения, выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e017-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="6e017-122">Фаиледсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="6e017-122">failedSignInCount</span></span>|<span data-ttu-id="6e017-123">Int64</span><span class="sxs-lookup"><span data-stu-id="6e017-123">Int64</span></span>|<span data-ttu-id="6e017-124">Количество неудачных операций входа, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="6e017-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="6e017-125">Сукцессперцентаже</span><span class="sxs-lookup"><span data-stu-id="6e017-125">successPercentage</span></span>|<span data-ttu-id="6e017-126">Int32</span><span class="sxs-lookup"><span data-stu-id="6e017-126">Int32</span></span>|<span data-ttu-id="6e017-127">Процент успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="6e017-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="6e017-128">Сукцессфулсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="6e017-128">successfulSignInCount</span></span>|<span data-ttu-id="6e017-129">Int64</span><span class="sxs-lookup"><span data-stu-id="6e017-129">Int64</span></span>|<span data-ttu-id="6e017-130">Количество успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="6e017-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e017-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="6e017-131">Relationships</span></span>
<span data-ttu-id="6e017-132">Нет</span><span class="sxs-lookup"><span data-stu-id="6e017-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e017-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e017-133">JSON representation</span></span>

<span data-ttu-id="6e017-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e017-134">The following is a JSON representation of the resource.</span></span>

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
