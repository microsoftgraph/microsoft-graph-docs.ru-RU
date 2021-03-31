---
title: тип ресурса appConsentRequest
description: Запрос, который представляет собой агрегацию userConsentRequests для определенного приложения.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ac7e9f2ea8e727a285016641bac10ea3d2e38f9b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469645"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="83e24-103">тип ресурса appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="83e24-103">appConsentRequest resource type</span></span>

<span data-ttu-id="83e24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83e24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83e24-105">Aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.</span><span class="sxs-lookup"><span data-stu-id="83e24-105">An aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="83e24-106">Методы</span><span class="sxs-lookup"><span data-stu-id="83e24-106">Methods</span></span>

|<span data-ttu-id="83e24-107">Метод</span><span class="sxs-lookup"><span data-stu-id="83e24-107">Method</span></span>|<span data-ttu-id="83e24-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="83e24-108">Return type</span></span>|<span data-ttu-id="83e24-109">Описание</span><span class="sxs-lookup"><span data-stu-id="83e24-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83e24-110">Список appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="83e24-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="83e24-111">[коллекция appConsentRequest](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="83e24-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="83e24-112">Получите список объектов [appConsentRequest](../resources/appconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="83e24-112">Get a list of the [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="83e24-113">Get appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="83e24-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="83e24-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="83e24-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="83e24-115">Ознакомьтесь с свойствами и отношениями [объекта appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="83e24-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="83e24-116">appConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="83e24-116">appConsentRequests: filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="83e24-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="83e24-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="83e24-118">Список [appConsentRequests,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом</span><span class="sxs-lookup"><span data-stu-id="83e24-118">A list of the [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer</span></span>|

## <a name="properties"></a><span data-ttu-id="83e24-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="83e24-119">Properties</span></span>

|<span data-ttu-id="83e24-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="83e24-120">Property</span></span>|<span data-ttu-id="83e24-121">Тип</span><span class="sxs-lookup"><span data-stu-id="83e24-121">Type</span></span>|<span data-ttu-id="83e24-122">Описание</span><span class="sxs-lookup"><span data-stu-id="83e24-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83e24-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="83e24-123">appDisplayName</span></span>|<span data-ttu-id="83e24-124">String</span><span class="sxs-lookup"><span data-stu-id="83e24-124">String</span></span>|<span data-ttu-id="83e24-125">Отображение имени приложения, для которого запрашивается согласие.</span><span class="sxs-lookup"><span data-stu-id="83e24-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="83e24-126">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="83e24-126">Required.</span></span> <span data-ttu-id="83e24-127">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="83e24-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="83e24-128">appId</span><span class="sxs-lookup"><span data-stu-id="83e24-128">appId</span></span>|<span data-ttu-id="83e24-129">String</span><span class="sxs-lookup"><span data-stu-id="83e24-129">String</span></span>|<span data-ttu-id="83e24-130">Идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="83e24-130">The identifier of the application.</span></span> <span data-ttu-id="83e24-131">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="83e24-131">Required.</span></span> <span data-ttu-id="83e24-132">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="83e24-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="83e24-133">id</span><span class="sxs-lookup"><span data-stu-id="83e24-133">id</span></span>|<span data-ttu-id="83e24-134">String</span><span class="sxs-lookup"><span data-stu-id="83e24-134">String</span></span>|<span data-ttu-id="83e24-135">Идентификатор запроса на согласие приложения.</span><span class="sxs-lookup"><span data-stu-id="83e24-135">The identifier of the app consent request.</span></span> <span data-ttu-id="83e24-136">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="83e24-136">Required.</span></span>|
|<span data-ttu-id="83e24-137">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="83e24-137">pendingScopes</span></span>|<span data-ttu-id="83e24-138">[коллекция appConsentRequestScope](../resources/appconsentrequestscope.md)</span><span class="sxs-lookup"><span data-stu-id="83e24-138">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="83e24-139">Список ожидающих утверждения областей.</span><span class="sxs-lookup"><span data-stu-id="83e24-139">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="83e24-140">Это пусто, если consentType `Static` .</span><span class="sxs-lookup"><span data-stu-id="83e24-140">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="83e24-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83e24-141">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83e24-142">Связи</span><span class="sxs-lookup"><span data-stu-id="83e24-142">Relationships</span></span>

|<span data-ttu-id="83e24-143">Связь</span><span class="sxs-lookup"><span data-stu-id="83e24-143">Relationship</span></span>|<span data-ttu-id="83e24-144">Тип</span><span class="sxs-lookup"><span data-stu-id="83e24-144">Type</span></span>|<span data-ttu-id="83e24-145">Описание</span><span class="sxs-lookup"><span data-stu-id="83e24-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83e24-146">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="83e24-146">userConsentRequests</span></span>|<span data-ttu-id="83e24-147">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="83e24-147">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="83e24-148">Список ожидающих запросов на согласие пользователей.</span><span class="sxs-lookup"><span data-stu-id="83e24-148">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83e24-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83e24-149">JSON representation</span></span>

<span data-ttu-id="83e24-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83e24-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```
