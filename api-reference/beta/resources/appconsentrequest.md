---
title: тип ресурса appConsentRequest
description: Запрос, представляюща коллекцию объектов userConsentRequest для определенного приложения.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d9c01fd4e752bca0fe9518553f52312e523da3a3
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697903"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="1bf9e-103">тип ресурса appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="1bf9e-103">appConsentRequest resource type</span></span>

<span data-ttu-id="1bf9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bf9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bf9e-105">Коллекция объектов [userConsentRequest](../resources/userconsentrequest.md) для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-105">A collection of [userConsentRequest](../resources/userconsentrequest.md) objects for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="1bf9e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1bf9e-106">Methods</span></span>
|<span data-ttu-id="1bf9e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1bf9e-107">Method</span></span>|<span data-ttu-id="1bf9e-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="1bf9e-108">Return type</span></span>|<span data-ttu-id="1bf9e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf9e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1bf9e-110">Список appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="1bf9e-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="1bf9e-111">[коллекция appConsentRequest](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="1bf9e-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="1bf9e-112">Извлечение коллекции [объектов appConsentRequest](appconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-112">Retrieve a collection of [appConsentRequest](appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="1bf9e-113">Get appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="1bf9e-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="1bf9e-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="1bf9e-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="1bf9e-115">Ознакомьтесь с свойствами и отношениями [объекта appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="1bf9e-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="1bf9e-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="1bf9e-116">filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="1bf9e-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="1bf9e-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="1bf9e-118">Ознакомьтесь с свойствами объектов [appConsentRequest,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом, и состояние запроса на согласие пользователя `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="1bf9e-118">Read the properties of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the user consent request is `InProgress`.</span></span>|

## <a name="properties"></a><span data-ttu-id="1bf9e-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bf9e-119">Properties</span></span>
|<span data-ttu-id="1bf9e-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bf9e-120">Property</span></span>|<span data-ttu-id="1bf9e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1bf9e-121">Type</span></span>|<span data-ttu-id="1bf9e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf9e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bf9e-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="1bf9e-123">appDisplayName</span></span>|<span data-ttu-id="1bf9e-124">String</span><span class="sxs-lookup"><span data-stu-id="1bf9e-124">String</span></span>|<span data-ttu-id="1bf9e-125">Отображение имени приложения, для которого запрашивается согласие.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="1bf9e-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-126">Required.</span></span> <span data-ttu-id="1bf9e-127">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="1bf9e-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="1bf9e-128">appId</span><span class="sxs-lookup"><span data-stu-id="1bf9e-128">appId</span></span>|<span data-ttu-id="1bf9e-129">String</span><span class="sxs-lookup"><span data-stu-id="1bf9e-129">String</span></span>|<span data-ttu-id="1bf9e-130">Идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-130">The identifier of the application.</span></span> <span data-ttu-id="1bf9e-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-131">Required.</span></span> <span data-ttu-id="1bf9e-132">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="1bf9e-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="1bf9e-133">consentType</span><span class="sxs-lookup"><span data-stu-id="1bf9e-133">consentType</span></span>|<span data-ttu-id="1bf9e-134">String</span><span class="sxs-lookup"><span data-stu-id="1bf9e-134">String</span></span>|<span data-ttu-id="1bf9e-135">Тип согласия запроса.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-135">The consent type of the request.</span></span> <span data-ttu-id="1bf9e-136">Возможные значения: `Static`   и  `Dynamic` .</span><span class="sxs-lookup"><span data-stu-id="1bf9e-136">Possible values are: `Static` and `Dynamic`.</span></span> <span data-ttu-id="1bf9e-137">Они представляют статические и динамические разрешения, соответственно, запрашиваются в рабочего процесса согласия.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-137">These represent static and dynamic permissions, respectively, requested in the consent workflow.</span></span> <span data-ttu-id="1bf9e-138">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="1bf9e-138">Supports `$filter` (`eq` only) and `$orderby`.</span></span> <span data-ttu-id="1bf9e-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-139">Required.</span></span>|
|<span data-ttu-id="1bf9e-140">id</span><span class="sxs-lookup"><span data-stu-id="1bf9e-140">id</span></span>|<span data-ttu-id="1bf9e-141">String</span><span class="sxs-lookup"><span data-stu-id="1bf9e-141">String</span></span>|<span data-ttu-id="1bf9e-142">Идентификатор запроса на согласие приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-142">The identifier of the app consent request.</span></span> <span data-ttu-id="1bf9e-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-143">Required.</span></span>|
|<span data-ttu-id="1bf9e-144">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="1bf9e-144">pendingScopes</span></span>|<span data-ttu-id="1bf9e-145">[коллекция appConsentRequestScope](../resources/appconsentrequestscope.md)</span><span class="sxs-lookup"><span data-stu-id="1bf9e-145">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="1bf9e-146">Список ожидающих утверждения областей.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-146">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="1bf9e-147">Это пусто, если consentType `Static` .</span><span class="sxs-lookup"><span data-stu-id="1bf9e-147">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="1bf9e-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-148">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bf9e-149">Связи</span><span class="sxs-lookup"><span data-stu-id="1bf9e-149">Relationships</span></span>
|<span data-ttu-id="1bf9e-150">Связь</span><span class="sxs-lookup"><span data-stu-id="1bf9e-150">Relationship</span></span>|<span data-ttu-id="1bf9e-151">Тип</span><span class="sxs-lookup"><span data-stu-id="1bf9e-151">Type</span></span>|<span data-ttu-id="1bf9e-152">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf9e-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bf9e-153">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="1bf9e-153">userConsentRequests</span></span>|<span data-ttu-id="1bf9e-154">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="1bf9e-154">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="1bf9e-155">Список ожидающих запросов на согласие пользователей.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-155">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1bf9e-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bf9e-156">JSON representation</span></span>
<span data-ttu-id="1bf9e-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bf9e-157">The following is a JSON representation of the resource.</span></span>
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

