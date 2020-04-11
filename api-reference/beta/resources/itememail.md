---
title: Тип ресурса Итемемаил
description: Тип ресурса Итемемаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aaf58bd7e20caeb418946814daa7ca8f7bb9bfa3
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229418"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="f9219-103">Тип ресурса Итемемаил</span><span class="sxs-lookup"><span data-stu-id="f9219-103">itemEmail resource type</span></span>

<span data-ttu-id="f9219-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9219-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9219-105">Представляет подробные сведения об адресах электронной почты, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f9219-105">Represents detailed information about email addresses associated with the user.</span></span>

## <a name="methods"></a><span data-ttu-id="f9219-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f9219-106">Methods</span></span>

| <span data-ttu-id="f9219-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f9219-107">Method</span></span>                                   | <span data-ttu-id="f9219-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f9219-108">Return Type</span></span>               | <span data-ttu-id="f9219-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f9219-109">Description</span></span>                                                      |
|:-----------------------------------------|:--------------------------|:-----------------------------------------------------------------|
| <span data-ttu-id="f9219-110">[получение](../api/itememail-get.md);</span><span class="sxs-lookup"><span data-stu-id="f9219-110">[Get](../api/itememail-get.md)</span></span>           | [<span data-ttu-id="f9219-111">итемемаил</span><span class="sxs-lookup"><span data-stu-id="f9219-111">itemEmail</span></span>](itememail.md) | <span data-ttu-id="f9219-112">Чтение свойств и связей объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="f9219-112">Read properties and relationships of an **itemEmail** object.</span></span>    |
| [<span data-ttu-id="f9219-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="f9219-113">Update</span></span>](../api/itememail-update.md)     | [<span data-ttu-id="f9219-114">итемемаил</span><span class="sxs-lookup"><span data-stu-id="f9219-114">itemEmail</span></span>](itememail.md) | <span data-ttu-id="f9219-115">Обновление объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="f9219-115">Update an **itemEmail** object.</span></span>                                  |
| [<span data-ttu-id="f9219-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="f9219-116">Delete</span></span>](../api/itememail-delete.md)     | <span data-ttu-id="f9219-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f9219-117">None</span></span>                      | <span data-ttu-id="f9219-118">Удаление объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="f9219-118">Delete an **itemEmail** object.</span></span>                                  |

## <a name="properties"></a><span data-ttu-id="f9219-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9219-119">Properties</span></span>

| <span data-ttu-id="f9219-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9219-120">Property</span></span>     | <span data-ttu-id="f9219-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f9219-121">Type</span></span>        | <span data-ttu-id="f9219-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f9219-122">Description</span></span>                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|<span data-ttu-id="f9219-123">address</span><span class="sxs-lookup"><span data-stu-id="f9219-123">address</span></span>       |<span data-ttu-id="f9219-124">String</span><span class="sxs-lookup"><span data-stu-id="f9219-124">String</span></span>       | <span data-ttu-id="f9219-125">Сам адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f9219-125">The email address itself.</span></span>                                                 |
|<span data-ttu-id="f9219-126">displayName</span><span class="sxs-lookup"><span data-stu-id="f9219-126">displayName</span></span>   |<span data-ttu-id="f9219-127">Строка</span><span class="sxs-lookup"><span data-stu-id="f9219-127">String</span></span>       | <span data-ttu-id="f9219-128">Имя или метка, с которыми пользователь связан с определенным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f9219-128">The name or label a user has associated with a particular email address.</span></span>  |
|<span data-ttu-id="f9219-129">type</span><span class="sxs-lookup"><span data-stu-id="f9219-129">type</span></span>          |<span data-ttu-id="f9219-130">строка</span><span class="sxs-lookup"><span data-stu-id="f9219-130">string</span></span>       | <span data-ttu-id="f9219-131">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="f9219-131">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>      |

## <a name="relationships"></a><span data-ttu-id="f9219-132">Связи</span><span class="sxs-lookup"><span data-stu-id="f9219-132">Relationships</span></span>

<span data-ttu-id="f9219-133">Нет</span><span class="sxs-lookup"><span data-stu-id="f9219-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9219-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9219-134">JSON representation</span></span>

<span data-ttu-id="f9219-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9219-135">The following is a JSON representation of the resource.</span></span>

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
