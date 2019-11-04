---
title: Тип ресурса Итемемаил
description: Тип ресурса Итемемаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: eed73f61b281463848c8520ebdcdbc75ac26d29d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939336"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="81012-103">Тип ресурса Итемемаил</span><span class="sxs-lookup"><span data-stu-id="81012-103">itemEmail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81012-104">Представляет подробные сведения об адресах электронной почты, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="81012-104">Represents detailed information about email addresses associated with the user.</span></span>

## <a name="methods"></a><span data-ttu-id="81012-105">Методы</span><span class="sxs-lookup"><span data-stu-id="81012-105">Methods</span></span>

| <span data-ttu-id="81012-106">Метод</span><span class="sxs-lookup"><span data-stu-id="81012-106">Method</span></span>                                   | <span data-ttu-id="81012-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81012-107">Return Type</span></span>               | <span data-ttu-id="81012-108">Описание</span><span class="sxs-lookup"><span data-stu-id="81012-108">Description</span></span>                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="81012-109">Получение</span><span class="sxs-lookup"><span data-stu-id="81012-109">Get</span></span>](../api/itememail-get.md) | [<span data-ttu-id="81012-110">итемемаил</span><span class="sxs-lookup"><span data-stu-id="81012-110">itemEmail</span></span>](itememail.md) | <span data-ttu-id="81012-111">Чтение свойств и связей объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="81012-111">Read properties and relationships of an **itemEmail** object.</span></span> |
| [<span data-ttu-id="81012-112">Update</span><span class="sxs-lookup"><span data-stu-id="81012-112">Update</span></span>](../api/itememail-update.md)     | [<span data-ttu-id="81012-113">итемемаил</span><span class="sxs-lookup"><span data-stu-id="81012-113">itemEmail</span></span>](itememail.md) | <span data-ttu-id="81012-114">Обновление объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="81012-114">Update an **itemEmail** object.</span></span>                               |
| [<span data-ttu-id="81012-115">Delete</span><span class="sxs-lookup"><span data-stu-id="81012-115">Delete</span></span>](../api/itememail-delete.md)     | <span data-ttu-id="81012-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="81012-116">None</span></span>                      | <span data-ttu-id="81012-117">Удаление объекта **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="81012-117">Delete an **itemEmail** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="81012-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="81012-118">Properties</span></span>

| <span data-ttu-id="81012-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="81012-119">Property</span></span>     | <span data-ttu-id="81012-120">Тип</span><span class="sxs-lookup"><span data-stu-id="81012-120">Type</span></span>        | <span data-ttu-id="81012-121">Описание</span><span class="sxs-lookup"><span data-stu-id="81012-121">Description</span></span>                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|<span data-ttu-id="81012-122">address</span><span class="sxs-lookup"><span data-stu-id="81012-122">address</span></span>       |<span data-ttu-id="81012-123">String</span><span class="sxs-lookup"><span data-stu-id="81012-123">String</span></span>       | <span data-ttu-id="81012-124">Сам адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="81012-124">The email address itself.</span></span>                                                 |
|<span data-ttu-id="81012-125">displayName</span><span class="sxs-lookup"><span data-stu-id="81012-125">displayName</span></span>   |<span data-ttu-id="81012-126">Строка</span><span class="sxs-lookup"><span data-stu-id="81012-126">String</span></span>       | <span data-ttu-id="81012-127">Имя или метка, с которыми пользователь связан с определенным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="81012-127">The name or label a user has associated with a particular email address.</span></span>  |
|<span data-ttu-id="81012-128">type</span><span class="sxs-lookup"><span data-stu-id="81012-128">type</span></span>          |<span data-ttu-id="81012-129">строка</span><span class="sxs-lookup"><span data-stu-id="81012-129">string</span></span>       | <span data-ttu-id="81012-130">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="81012-130">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>      |

## <a name="relationships"></a><span data-ttu-id="81012-131">Связи</span><span class="sxs-lookup"><span data-stu-id="81012-131">Relationships</span></span>

<span data-ttu-id="81012-132">Нет</span><span class="sxs-lookup"><span data-stu-id="81012-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81012-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81012-133">JSON representation</span></span>

<span data-ttu-id="81012-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81012-134">The following is a JSON representation of the resource.</span></span>

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
