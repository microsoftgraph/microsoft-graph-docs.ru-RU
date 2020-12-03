---
title: Тип ресурса Аппликатионсигниндетаиледсуммари
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: abe2d8524d2ef23885285bacc0c953057035f54d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523814"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="85efc-103">Тип ресурса Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="85efc-103">applicationSignInSummary resource type</span></span>

<span data-ttu-id="85efc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85efc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85efc-105">Представляет сводку по входу в приложение.</span><span class="sxs-lookup"><span data-stu-id="85efc-105">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="85efc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="85efc-106">Methods</span></span>

| <span data-ttu-id="85efc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="85efc-107">Method</span></span>       | <span data-ttu-id="85efc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85efc-108">Return Type</span></span> | <span data-ttu-id="85efc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="85efc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="85efc-110">Получение Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="85efc-110">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="85efc-111">аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="85efc-111">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="85efc-112">Чтение свойств и связей объекта **аппликатионсигнинсуммари** .</span><span class="sxs-lookup"><span data-stu-id="85efc-112">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="85efc-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="85efc-113">Properties</span></span>
| <span data-ttu-id="85efc-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="85efc-114">Property</span></span>     | <span data-ttu-id="85efc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="85efc-115">Type</span></span>        | <span data-ttu-id="85efc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="85efc-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="85efc-117">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="85efc-117">appDisplayName</span></span>|<span data-ttu-id="85efc-118">String</span><span class="sxs-lookup"><span data-stu-id="85efc-118">String</span></span>|<span data-ttu-id="85efc-119">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="85efc-119">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="85efc-120">appId</span><span class="sxs-lookup"><span data-stu-id="85efc-120">appId</span></span>|<span data-ttu-id="85efc-121">String</span><span class="sxs-lookup"><span data-stu-id="85efc-121">String</span></span>|  <span data-ttu-id="85efc-122">Идентификатор приложения, выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="85efc-122">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="85efc-123">фаиледсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="85efc-123">failedSignInCount</span></span>|<span data-ttu-id="85efc-124">Int64</span><span class="sxs-lookup"><span data-stu-id="85efc-124">Int64</span></span>|<span data-ttu-id="85efc-125">Количество неудачных операций входа, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="85efc-125">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="85efc-126">сукцессперцентаже</span><span class="sxs-lookup"><span data-stu-id="85efc-126">successPercentage</span></span>|<span data-ttu-id="85efc-127">Int32</span><span class="sxs-lookup"><span data-stu-id="85efc-127">Int32</span></span>|<span data-ttu-id="85efc-128">Процент успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="85efc-128">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="85efc-129">сукцессфулсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="85efc-129">successfulSignInCount</span></span>|<span data-ttu-id="85efc-130">Int64</span><span class="sxs-lookup"><span data-stu-id="85efc-130">Int64</span></span>|<span data-ttu-id="85efc-131">Количество успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="85efc-131">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85efc-132">Связи</span><span class="sxs-lookup"><span data-stu-id="85efc-132">Relationships</span></span>
<span data-ttu-id="85efc-133">Нет</span><span class="sxs-lookup"><span data-stu-id="85efc-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="85efc-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85efc-134">JSON representation</span></span>

<span data-ttu-id="85efc-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85efc-135">The following is a JSON representation of the resource.</span></span>

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


