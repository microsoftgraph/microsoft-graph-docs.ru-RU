---
title: Тип ресурса Итемемаил
description: Тип ресурса Итемемаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a18d72fb44f373b6cee1047cc2eed5f0c18a1d0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523081"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="476f2-103">Тип ресурса Итемемаил</span><span class="sxs-lookup"><span data-stu-id="476f2-103">itemEmail resource type</span></span>

<span data-ttu-id="476f2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="476f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="476f2-105">Представляет подробные сведения об адресах электронной почты, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="476f2-105">Represents detailed information about email addresses associated with the user.</span></span>

## <a name="methods"></a><span data-ttu-id="476f2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="476f2-106">Methods</span></span>

| <span data-ttu-id="476f2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="476f2-107">Method</span></span>                                   | <span data-ttu-id="476f2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="476f2-108">Return Type</span></span>               | <span data-ttu-id="476f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="476f2-109">Description</span></span>                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| <span data-ttu-id="476f2-110">[получение](../api/itememail-get.md);</span><span class="sxs-lookup"><span data-stu-id="476f2-110">[Get](../api/itememail-get.md)</span></span> | [<span data-ttu-id="476f2-111">итемемаил</span><span class="sxs-lookup"><span data-stu-id="476f2-111">itemEmail</span></span>](itememail.md) | <span data-ttu-id="476f2-112">Чтение свойств и связей объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="476f2-112">Read properties and relationships of an **itemEmail** object.</span></span> |
| <span data-ttu-id="476f2-113">[обновление](../api/itememail-update.md).</span><span class="sxs-lookup"><span data-stu-id="476f2-113">[Update](../api/itememail-update.md)</span></span>     | [<span data-ttu-id="476f2-114">итемемаил</span><span class="sxs-lookup"><span data-stu-id="476f2-114">itemEmail</span></span>](itememail.md) | <span data-ttu-id="476f2-115">Обновление объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="476f2-115">Update an **itemEmail** object.</span></span>                               |
| <span data-ttu-id="476f2-116">[удаление](../api/itememail-delete.md);</span><span class="sxs-lookup"><span data-stu-id="476f2-116">[Delete](../api/itememail-delete.md)</span></span>     | <span data-ttu-id="476f2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="476f2-117">None</span></span>                      | <span data-ttu-id="476f2-118">Удаление объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="476f2-118">Delete an **itemEmail** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="476f2-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="476f2-119">Properties</span></span>

| <span data-ttu-id="476f2-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="476f2-120">Property</span></span>     | <span data-ttu-id="476f2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="476f2-121">Type</span></span>        | <span data-ttu-id="476f2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="476f2-122">Description</span></span>                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|<span data-ttu-id="476f2-123">address</span><span class="sxs-lookup"><span data-stu-id="476f2-123">address</span></span>       |<span data-ttu-id="476f2-124">String</span><span class="sxs-lookup"><span data-stu-id="476f2-124">String</span></span>       | <span data-ttu-id="476f2-125">Сам адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="476f2-125">The email address itself.</span></span>                                                 |
|<span data-ttu-id="476f2-126">displayName</span><span class="sxs-lookup"><span data-stu-id="476f2-126">displayName</span></span>   |<span data-ttu-id="476f2-127">Строка</span><span class="sxs-lookup"><span data-stu-id="476f2-127">String</span></span>       | <span data-ttu-id="476f2-128">Имя или метка, с которыми пользователь связан с определенным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="476f2-128">The name or label a user has associated with a particular email address.</span></span>  |
|<span data-ttu-id="476f2-129">type</span><span class="sxs-lookup"><span data-stu-id="476f2-129">type</span></span>          |<span data-ttu-id="476f2-130">строка</span><span class="sxs-lookup"><span data-stu-id="476f2-130">string</span></span>       | <span data-ttu-id="476f2-131">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="476f2-131">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>      |

## <a name="relationships"></a><span data-ttu-id="476f2-132">Связи</span><span class="sxs-lookup"><span data-stu-id="476f2-132">Relationships</span></span>

<span data-ttu-id="476f2-133">Нет</span><span class="sxs-lookup"><span data-stu-id="476f2-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="476f2-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="476f2-134">JSON representation</span></span>

<span data-ttu-id="476f2-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="476f2-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": ""
}-->

```json
{
  "address": "String",
  "displayName": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemEmail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
