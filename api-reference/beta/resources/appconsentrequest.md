---
title: тип ресурса appConsentRequest
description: Запрос, который представляет собой агрегацию userConsentRequests для определенного приложения.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f823f64d4c0324aeca74c3268d6fc95d313e2f00
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965235"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="9eea5-103">тип ресурса appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="9eea5-103">appConsentRequest resource type</span></span>

<span data-ttu-id="9eea5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eea5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9eea5-105">Aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.</span><span class="sxs-lookup"><span data-stu-id="9eea5-105">An aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="9eea5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9eea5-106">Methods</span></span>
|<span data-ttu-id="9eea5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9eea5-107">Method</span></span>|<span data-ttu-id="9eea5-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="9eea5-108">Return type</span></span>|<span data-ttu-id="9eea5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9eea5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9eea5-110">Список appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="9eea5-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="9eea5-111">[коллекция appConsentRequest](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9eea5-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="9eea5-112">Получите список объектов [appConsentRequest](../resources/appconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="9eea5-112">Get a list of the [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="9eea5-113">Get appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="9eea5-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="9eea5-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="9eea5-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="9eea5-115">Ознакомьтесь с свойствами и отношениями [объекта appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9eea5-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="9eea5-116">Список appConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="9eea5-116">List appConsentRequests: filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="9eea5-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="9eea5-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="9eea5-118">Список [appConsentRequests,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом</span><span class="sxs-lookup"><span data-stu-id="9eea5-118">A list of the [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer</span></span>|

## <a name="properties"></a><span data-ttu-id="9eea5-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="9eea5-119">Properties</span></span>
|<span data-ttu-id="9eea5-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="9eea5-120">Property</span></span>|<span data-ttu-id="9eea5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9eea5-121">Type</span></span>|<span data-ttu-id="9eea5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9eea5-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eea5-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="9eea5-123">appDisplayName</span></span>|<span data-ttu-id="9eea5-124">String</span><span class="sxs-lookup"><span data-stu-id="9eea5-124">String</span></span>|<span data-ttu-id="9eea5-125">Отображение имени приложения, для которого запрашивается согласие.</span><span class="sxs-lookup"><span data-stu-id="9eea5-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="9eea5-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9eea5-126">Required.</span></span> <span data-ttu-id="9eea5-127">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="9eea5-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="9eea5-128">appId</span><span class="sxs-lookup"><span data-stu-id="9eea5-128">appId</span></span>|<span data-ttu-id="9eea5-129">String</span><span class="sxs-lookup"><span data-stu-id="9eea5-129">String</span></span>|<span data-ttu-id="9eea5-130">Идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="9eea5-130">The identifier of the application.</span></span> <span data-ttu-id="9eea5-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9eea5-131">Required.</span></span> <span data-ttu-id="9eea5-132">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="9eea5-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="9eea5-133">consentType</span><span class="sxs-lookup"><span data-stu-id="9eea5-133">consentType</span></span>|<span data-ttu-id="9eea5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9eea5-134">String</span></span>|<span data-ttu-id="9eea5-135">Тип согласия запроса.</span><span class="sxs-lookup"><span data-stu-id="9eea5-135">The consent type of the request.</span></span> <span data-ttu-id="9eea5-136">Возможные значения: `Static`   и  `Dynamic` .</span><span class="sxs-lookup"><span data-stu-id="9eea5-136">Possible values are: `Static` and `Dynamic`.</span></span> <span data-ttu-id="9eea5-137">Они представляют статические и динамические разрешения, соответственно, запрашиваются в рабочего процесса согласия.</span><span class="sxs-lookup"><span data-stu-id="9eea5-137">These represent static and dynamic permissions, respectively, requested in the consent workflow.</span></span> <span data-ttu-id="9eea5-138">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="9eea5-138">Supports `$filter` (`eq` only) and `$orderby`.</span></span> <span data-ttu-id="9eea5-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9eea5-139">Required.</span></span>|
|<span data-ttu-id="9eea5-140">id</span><span class="sxs-lookup"><span data-stu-id="9eea5-140">id</span></span>|<span data-ttu-id="9eea5-141">Строка</span><span class="sxs-lookup"><span data-stu-id="9eea5-141">String</span></span>|<span data-ttu-id="9eea5-142">Идентификатор запроса на согласие приложения.</span><span class="sxs-lookup"><span data-stu-id="9eea5-142">The identifier of the app consent request.</span></span> <span data-ttu-id="9eea5-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9eea5-143">Required.</span></span>|
|<span data-ttu-id="9eea5-144">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="9eea5-144">pendingScopes</span></span>|<span data-ttu-id="9eea5-145">[коллекция appConsentRequestScope](../resources/appconsentrequestscope.md)</span><span class="sxs-lookup"><span data-stu-id="9eea5-145">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="9eea5-146">Список ожидающих утверждения областей.</span><span class="sxs-lookup"><span data-stu-id="9eea5-146">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="9eea5-147">Это пусто, если consentType `Static` .</span><span class="sxs-lookup"><span data-stu-id="9eea5-147">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="9eea5-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9eea5-148">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9eea5-149">Связи</span><span class="sxs-lookup"><span data-stu-id="9eea5-149">Relationships</span></span>
|<span data-ttu-id="9eea5-150">Связь</span><span class="sxs-lookup"><span data-stu-id="9eea5-150">Relationship</span></span>|<span data-ttu-id="9eea5-151">Тип</span><span class="sxs-lookup"><span data-stu-id="9eea5-151">Type</span></span>|<span data-ttu-id="9eea5-152">Описание</span><span class="sxs-lookup"><span data-stu-id="9eea5-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eea5-153">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="9eea5-153">userConsentRequests</span></span>|<span data-ttu-id="9eea5-154">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9eea5-154">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="9eea5-155">Список ожидающих запросов на согласие пользователей.</span><span class="sxs-lookup"><span data-stu-id="9eea5-155">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9eea5-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9eea5-156">JSON representation</span></span>
<span data-ttu-id="9eea5-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9eea5-157">The following is a JSON representation of the resource.</span></span>
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
  "consentType": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```

