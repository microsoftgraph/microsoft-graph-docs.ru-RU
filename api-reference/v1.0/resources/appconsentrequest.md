---
title: тип ресурса appConsentRequest
description: Запрос, представляюща коллекцию объектов userConsentRequest для определенного приложения.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 32744ce01f871c82a52710502e7fdc899537cef5
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698015"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="aabbe-103">тип ресурса appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="aabbe-103">appConsentRequest resource type</span></span>

<span data-ttu-id="aabbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aabbe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aabbe-105">Коллекция объектов [userConsentRequest](../resources/userconsentrequest.md) для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="aabbe-105">A collection of [userConsentRequest](../resources/userconsentrequest.md) objects for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="aabbe-106">Методы</span><span class="sxs-lookup"><span data-stu-id="aabbe-106">Methods</span></span>

|<span data-ttu-id="aabbe-107">Метод</span><span class="sxs-lookup"><span data-stu-id="aabbe-107">Method</span></span>|<span data-ttu-id="aabbe-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="aabbe-108">Return type</span></span>|<span data-ttu-id="aabbe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aabbe-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aabbe-110">Список appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="aabbe-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="aabbe-111">[коллекция appConsentRequest](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="aabbe-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="aabbe-112">Извлечение коллекции [объектов appConsentRequest](appconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="aabbe-112">Retrieve a collection of [appConsentRequest](appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="aabbe-113">Get appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="aabbe-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="aabbe-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="aabbe-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="aabbe-115">Ознакомьтесь с свойствами и отношениями [объекта appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="aabbe-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="aabbe-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="aabbe-116">filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="aabbe-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="aabbe-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="aabbe-118">Ознакомьтесь с свойствами объектов [appConsentRequest,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом, и состояние запроса на согласие пользователя `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="aabbe-118">Read the properties of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the user consent request is `InProgress`.</span></span> |

## <a name="properties"></a><span data-ttu-id="aabbe-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="aabbe-119">Properties</span></span>

|<span data-ttu-id="aabbe-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="aabbe-120">Property</span></span>|<span data-ttu-id="aabbe-121">Тип</span><span class="sxs-lookup"><span data-stu-id="aabbe-121">Type</span></span>|<span data-ttu-id="aabbe-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aabbe-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aabbe-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="aabbe-123">appDisplayName</span></span>|<span data-ttu-id="aabbe-124">String</span><span class="sxs-lookup"><span data-stu-id="aabbe-124">String</span></span>|<span data-ttu-id="aabbe-125">Отображение имени приложения, для которого запрашивается согласие.</span><span class="sxs-lookup"><span data-stu-id="aabbe-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="aabbe-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aabbe-126">Required.</span></span> <span data-ttu-id="aabbe-127">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="aabbe-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="aabbe-128">appId</span><span class="sxs-lookup"><span data-stu-id="aabbe-128">appId</span></span>|<span data-ttu-id="aabbe-129">String</span><span class="sxs-lookup"><span data-stu-id="aabbe-129">String</span></span>|<span data-ttu-id="aabbe-130">Идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="aabbe-130">The identifier of the application.</span></span> <span data-ttu-id="aabbe-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aabbe-131">Required.</span></span> <span data-ttu-id="aabbe-132">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="aabbe-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="aabbe-133">id</span><span class="sxs-lookup"><span data-stu-id="aabbe-133">id</span></span>|<span data-ttu-id="aabbe-134">String</span><span class="sxs-lookup"><span data-stu-id="aabbe-134">String</span></span>|<span data-ttu-id="aabbe-135">Идентификатор запроса на согласие приложения.</span><span class="sxs-lookup"><span data-stu-id="aabbe-135">The identifier of the app consent request.</span></span> <span data-ttu-id="aabbe-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aabbe-136">Required.</span></span>|
|<span data-ttu-id="aabbe-137">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="aabbe-137">pendingScopes</span></span>|<span data-ttu-id="aabbe-138">[коллекция appConsentRequestScope](../resources/appconsentrequestscope.md)</span><span class="sxs-lookup"><span data-stu-id="aabbe-138">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="aabbe-139">Список ожидающих утверждения областей.</span><span class="sxs-lookup"><span data-stu-id="aabbe-139">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="aabbe-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aabbe-140">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aabbe-141">Связи</span><span class="sxs-lookup"><span data-stu-id="aabbe-141">Relationships</span></span>

|<span data-ttu-id="aabbe-142">Связь</span><span class="sxs-lookup"><span data-stu-id="aabbe-142">Relationship</span></span>|<span data-ttu-id="aabbe-143">Тип</span><span class="sxs-lookup"><span data-stu-id="aabbe-143">Type</span></span>|<span data-ttu-id="aabbe-144">Описание</span><span class="sxs-lookup"><span data-stu-id="aabbe-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aabbe-145">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="aabbe-145">userConsentRequests</span></span>|<span data-ttu-id="aabbe-146">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="aabbe-146">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="aabbe-147">Список ожидающих запросов на согласие пользователей.</span><span class="sxs-lookup"><span data-stu-id="aabbe-147">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aabbe-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aabbe-148">JSON representation</span></span>

<span data-ttu-id="aabbe-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aabbe-149">The following is a JSON representation of the resource.</span></span>
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
