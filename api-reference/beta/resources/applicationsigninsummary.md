---
title: Тип ресурса Аппликатионсигниндетаиледсуммари
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0329aec304602151a23ff389bc041247f9fb65b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32655393"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="e0ac1-103">Тип ресурса Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="e0ac1-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0ac1-104">Представляет сводку по входу в приложение.</span><span class="sxs-lookup"><span data-stu-id="e0ac1-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="e0ac1-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e0ac1-105">Methods</span></span>

| <span data-ttu-id="e0ac1-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e0ac1-106">Method</span></span>       | <span data-ttu-id="e0ac1-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e0ac1-107">Return Type</span></span> | <span data-ttu-id="e0ac1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e0ac1-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e0ac1-109">Получение Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="e0ac1-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="e0ac1-110">Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="e0ac1-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="e0ac1-111">Чтение свойств и связей объекта **аппликатионсигнинсуммари** .</span><span class="sxs-lookup"><span data-stu-id="e0ac1-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e0ac1-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0ac1-112">Properties</span></span>
| <span data-ttu-id="e0ac1-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0ac1-113">Property</span></span>     | <span data-ttu-id="e0ac1-114">Тип</span><span class="sxs-lookup"><span data-stu-id="e0ac1-114">Type</span></span>        | <span data-ttu-id="e0ac1-115">Описание</span><span class="sxs-lookup"><span data-stu-id="e0ac1-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0ac1-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0ac1-116">appDisplayName</span></span>|<span data-ttu-id="e0ac1-117">String</span><span class="sxs-lookup"><span data-stu-id="e0ac1-117">String</span></span>|<span data-ttu-id="e0ac1-118">Имя приложения, в которое пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="e0ac1-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="e0ac1-119">appId</span><span class="sxs-lookup"><span data-stu-id="e0ac1-119">appId</span></span>|<span data-ttu-id="e0ac1-120">String</span><span class="sxs-lookup"><span data-stu-id="e0ac1-120">String</span></span>|  <span data-ttu-id="e0ac1-121">Идентификатор приложения, выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="e0ac1-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="e0ac1-122">Фаиледсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="e0ac1-122">failedSignInCount</span></span>|<span data-ttu-id="e0ac1-123">Int64</span><span class="sxs-lookup"><span data-stu-id="e0ac1-123">Int64</span></span>|<span data-ttu-id="e0ac1-124">Количество неудачных операций входа, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="e0ac1-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="e0ac1-125">Сукцессперцентаже</span><span class="sxs-lookup"><span data-stu-id="e0ac1-125">successPercentage</span></span>|<span data-ttu-id="e0ac1-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ac1-126">Int32</span></span>|<span data-ttu-id="e0ac1-127">Процент успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="e0ac1-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="e0ac1-128">Сукцессфулсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="e0ac1-128">successfulSignInCount</span></span>|<span data-ttu-id="e0ac1-129">Int64</span><span class="sxs-lookup"><span data-stu-id="e0ac1-129">Int64</span></span>|<span data-ttu-id="e0ac1-130">Количество успешных входов, выполненных приложением.</span><span class="sxs-lookup"><span data-stu-id="e0ac1-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0ac1-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="e0ac1-131">Relationships</span></span>
<span data-ttu-id="e0ac1-132">Нет</span><span class="sxs-lookup"><span data-stu-id="e0ac1-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e0ac1-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0ac1-133">JSON representation</span></span>

<span data-ttu-id="e0ac1-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0ac1-134">The following is a JSON representation of the resource.</span></span>

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
