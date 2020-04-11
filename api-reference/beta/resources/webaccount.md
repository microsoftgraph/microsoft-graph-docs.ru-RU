---
title: Тип ресурса "учетная запись"
description: Тип ресурса "учетная запись"
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dbdae8f0035e92b1c5b74c0ef3f842d2eb5af37a
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228868"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="58e65-103">Тип ресурса "учетная запись"</span><span class="sxs-lookup"><span data-stu-id="58e65-103">webAccount resource type</span></span>

<span data-ttu-id="58e65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58e65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e65-105">Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой [профиль](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="58e65-105">Represents web accounts the user has indicated they use or has added to their user [profile](profile.md).</span></span>

<span data-ttu-id="58e65-106">Этот тип ресурса наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="58e65-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="58e65-107">Методы</span><span class="sxs-lookup"><span data-stu-id="58e65-107">Methods</span></span>

| <span data-ttu-id="58e65-108">Метод</span><span class="sxs-lookup"><span data-stu-id="58e65-108">Method</span></span>                                                | <span data-ttu-id="58e65-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="58e65-109">Return Type</span></span>                 | <span data-ttu-id="58e65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58e65-110">Description</span></span>                                                       |
|:------------------------------------------------------|:----------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="58e65-111">Получение учетной записи службы</span><span class="sxs-lookup"><span data-stu-id="58e65-111">Get webAccount</span></span>](../api/webaccount-get.md)            | [<span data-ttu-id="58e65-112">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="58e65-112">webAccount</span></span>](webaccount.md) | <span data-ttu-id="58e65-113">Чтение свойств и связей объекта веб- **учетных записей** .</span><span class="sxs-lookup"><span data-stu-id="58e65-113">Read the properties and relationships of a **webAccount** object.</span></span> |
| [<span data-ttu-id="58e65-114">Обновление учетной записи</span><span class="sxs-lookup"><span data-stu-id="58e65-114">Update webAccount</span></span>](../api/webaccount-update.md)      | [<span data-ttu-id="58e65-115">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="58e65-115">webAccount</span></span>](webaccount.md) | <span data-ttu-id="58e65-116">Обновление объекта **учетной записи** .</span><span class="sxs-lookup"><span data-stu-id="58e65-116">Update a **webAccount** object.</span></span>                                   |
| [<span data-ttu-id="58e65-117">Удаление учетной записи службы</span><span class="sxs-lookup"><span data-stu-id="58e65-117">Delete webAccount</span></span>](../api/webaccount-delete.md)      | <span data-ttu-id="58e65-118">Нет</span><span class="sxs-lookup"><span data-stu-id="58e65-118">None</span></span>                        | <span data-ttu-id="58e65-119">Удаление объекта **учетной записи** .</span><span class="sxs-lookup"><span data-stu-id="58e65-119">Delete a **webAccount** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="58e65-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="58e65-120">Properties</span></span>

| <span data-ttu-id="58e65-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="58e65-121">Property</span></span>     | <span data-ttu-id="58e65-122">Тип</span><span class="sxs-lookup"><span data-stu-id="58e65-122">Type</span></span>                                      | <span data-ttu-id="58e65-123">Описание</span><span class="sxs-lookup"><span data-stu-id="58e65-123">Description</span></span>                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="58e65-124">description</span><span class="sxs-lookup"><span data-stu-id="58e65-124">description</span></span>   |<span data-ttu-id="58e65-125">String</span><span class="sxs-lookup"><span data-stu-id="58e65-125">String</span></span>                                     | <span data-ttu-id="58e65-126">Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.</span><span class="sxs-lookup"><span data-stu-id="58e65-126">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="58e65-127">service</span><span class="sxs-lookup"><span data-stu-id="58e65-127">service</span></span>       |[<span data-ttu-id="58e65-128">сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="58e65-128">serviceInformation</span></span>](serviceinformation.md)| <span data-ttu-id="58e65-129">Содержит основные сведения о связанной службе.</span><span class="sxs-lookup"><span data-stu-id="58e65-129">Contains basic detail about the service that is being associated.</span></span>                              |
|<span data-ttu-id="58e65-130">статусмессаже</span><span class="sxs-lookup"><span data-stu-id="58e65-130">statusMessage</span></span> |<span data-ttu-id="58e65-131">String</span><span class="sxs-lookup"><span data-stu-id="58e65-131">String</span></span>                                     | <span data-ttu-id="58e65-132">Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано.</span><span class="sxs-lookup"><span data-stu-id="58e65-132">Contains a status message from the cloud service if provided or synchronized.</span></span>                  |
|<span data-ttu-id="58e65-133">userId</span><span class="sxs-lookup"><span data-stu-id="58e65-133">userId</span></span>        |<span data-ttu-id="58e65-134">String</span><span class="sxs-lookup"><span data-stu-id="58e65-134">String</span></span>                                     | <span data-ttu-id="58e65-135">Имя пользователя, отображаемое для учетной записи Account.</span><span class="sxs-lookup"><span data-stu-id="58e65-135">The user name  displayed for the webaccount.</span></span>                                                   |
|<span data-ttu-id="58e65-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="58e65-136">webUrl</span></span>        |<span data-ttu-id="58e65-137">String</span><span class="sxs-lookup"><span data-stu-id="58e65-137">String</span></span>                                     | <span data-ttu-id="58e65-138">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="58e65-138">Contains a link to the user's profile on the cloud service if one exists.</span></span>                      |

## <a name="relationships"></a><span data-ttu-id="58e65-139">Связи</span><span class="sxs-lookup"><span data-stu-id="58e65-139">Relationships</span></span>

<span data-ttu-id="58e65-140">Нет</span><span class="sxs-lookup"><span data-stu-id="58e65-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58e65-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58e65-141">JSON representation</span></span>

<span data-ttu-id="58e65-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58e65-142">The following is a JSON representation of the resource.</span></span>

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
