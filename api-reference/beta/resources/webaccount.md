---
title: Тип ресурса "учетная запись"
description: Тип ресурса "учетная запись"
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 414e3f491736f51ee670390519241110bc81f66e
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950357"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="b8c90-103">Тип ресурса "учетная запись"</span><span class="sxs-lookup"><span data-stu-id="b8c90-103">webAccount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8c90-104">Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой [профиль](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8c90-104">Represents web accounts the user has indicated they use or has added to their user [profile](profile.md).</span></span>

<span data-ttu-id="b8c90-105">Этот тип ресурса наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b8c90-105">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b8c90-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b8c90-106">Methods</span></span>

| <span data-ttu-id="b8c90-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b8c90-107">Method</span></span>                                     | <span data-ttu-id="b8c90-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b8c90-108">Return Type</span></span>                 | <span data-ttu-id="b8c90-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b8c90-109">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="b8c90-110">Получение учетной записи службы</span><span class="sxs-lookup"><span data-stu-id="b8c90-110">Get webAccount</span></span>](../api/webaccount-get.md) | [<span data-ttu-id="b8c90-111">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="b8c90-111">webAccount</span></span>](webaccount.md) | <span data-ttu-id="b8c90-112">Чтение свойств и связей объекта веб- **учетных записей** .</span><span class="sxs-lookup"><span data-stu-id="b8c90-112">Read the properties and relationships of a **webAccount** object.</span></span> |
| [<span data-ttu-id="b8c90-113">Обновление учетной записи</span><span class="sxs-lookup"><span data-stu-id="b8c90-113">Update webAccount</span></span>](../api/webaccount-update.md)      | [<span data-ttu-id="b8c90-114">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="b8c90-114">webAccount</span></span>](webaccount.md) | <span data-ttu-id="b8c90-115">Обновление объекта **учетной записи** .</span><span class="sxs-lookup"><span data-stu-id="b8c90-115">Update a **webAccount** object.</span></span>                               |
| [<span data-ttu-id="b8c90-116">Удаление учетной записи службы</span><span class="sxs-lookup"><span data-stu-id="b8c90-116">Delete webAccount</span></span>](../api/webaccount-delete.md)      | <span data-ttu-id="b8c90-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="b8c90-117">None</span></span>                        | <span data-ttu-id="b8c90-118">Удаление объекта **учетной записи** .</span><span class="sxs-lookup"><span data-stu-id="b8c90-118">Delete a **webAccount** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="b8c90-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8c90-119">Properties</span></span>

| <span data-ttu-id="b8c90-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8c90-120">Property</span></span>     | <span data-ttu-id="b8c90-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b8c90-121">Type</span></span>                                      | <span data-ttu-id="b8c90-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b8c90-122">Description</span></span>                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="b8c90-123">description</span><span class="sxs-lookup"><span data-stu-id="b8c90-123">description</span></span>   |<span data-ttu-id="b8c90-124">String</span><span class="sxs-lookup"><span data-stu-id="b8c90-124">String</span></span>                                     | <span data-ttu-id="b8c90-125">Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.</span><span class="sxs-lookup"><span data-stu-id="b8c90-125">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="b8c90-126">service</span><span class="sxs-lookup"><span data-stu-id="b8c90-126">service</span></span>       |[<span data-ttu-id="b8c90-127">сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="b8c90-127">serviceInformation</span></span>](serviceinformation.md)| <span data-ttu-id="b8c90-128">Содержит основные сведения о связанной службе.</span><span class="sxs-lookup"><span data-stu-id="b8c90-128">Contains basic detail about the service that is being associated.</span></span>                              |
|<span data-ttu-id="b8c90-129">статусмессаже</span><span class="sxs-lookup"><span data-stu-id="b8c90-129">statusMessage</span></span> |<span data-ttu-id="b8c90-130">String</span><span class="sxs-lookup"><span data-stu-id="b8c90-130">String</span></span>                                     | <span data-ttu-id="b8c90-131">Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано.</span><span class="sxs-lookup"><span data-stu-id="b8c90-131">Contains a status message from the cloud service if provided or synchronized.</span></span>                  |
|<span data-ttu-id="b8c90-132">userId</span><span class="sxs-lookup"><span data-stu-id="b8c90-132">userId</span></span>        |<span data-ttu-id="b8c90-133">String</span><span class="sxs-lookup"><span data-stu-id="b8c90-133">String</span></span>                                     | <span data-ttu-id="b8c90-134">Имя пользователя, отображаемое для учетной записи Account.</span><span class="sxs-lookup"><span data-stu-id="b8c90-134">The user name  displayed for the webaccount.</span></span>                                    |
|<span data-ttu-id="b8c90-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="b8c90-135">webUrl</span></span>        |<span data-ttu-id="b8c90-136">String</span><span class="sxs-lookup"><span data-stu-id="b8c90-136">String</span></span>                                     | <span data-ttu-id="b8c90-137">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="b8c90-137">Contains a link to the user's profile on the cloud service if one exists.</span></span>                       |

## <a name="relationships"></a><span data-ttu-id="b8c90-138">Связи</span><span class="sxs-lookup"><span data-stu-id="b8c90-138">Relationships</span></span>

<span data-ttu-id="b8c90-139">Нет</span><span class="sxs-lookup"><span data-stu-id="b8c90-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8c90-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8c90-140">JSON representation</span></span>

<span data-ttu-id="b8c90-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8c90-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": ""
}-->

```json
{
  "description": "String",
  "service": {"@odata.type": "microsoft.graph.serviceInformation"},
  "statusMessage": "String",
  "userId": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webAccount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
