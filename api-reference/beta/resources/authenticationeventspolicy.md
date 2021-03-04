---
title: тип ресурса authenticationEventsPolicy
description: События проверки подлинности используются для вызова потоков пользователей в определенных точках потока проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6cd727ebe51bbb6d5ad2162b180c4fc891ff792a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443169"
---
# <a name="authenticationeventspolicy-resource-type"></a><span data-ttu-id="28b0f-103">тип ресурса authenticationEventsPolicy</span><span class="sxs-lookup"><span data-stu-id="28b0f-103">authenticationEventsPolicy resource type</span></span>

<span data-ttu-id="28b0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28b0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b0f-105">Ресурс, который указывает события в опытом проверки подлинности, с каждым событием далее определяет доступные типы слушателей, которые могут быть созданы для события.</span><span class="sxs-lookup"><span data-stu-id="28b0f-105">A resource that specifies the events in the authentication experience, with each event further defining the available types of listeners that can be created for the event.</span></span> <span data-ttu-id="28b0f-106">События присущи опыту проверки подлинности; этот ресурс не настраивается пользователем.</span><span class="sxs-lookup"><span data-stu-id="28b0f-106">Events are inherent to the authentication experience; this resource is not user configurable.</span></span>

## <a name="methods"></a><span data-ttu-id="28b0f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="28b0f-107">Methods</span></span>

|<span data-ttu-id="28b0f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="28b0f-108">Method</span></span>|<span data-ttu-id="28b0f-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="28b0f-109">Return type</span></span>|<span data-ttu-id="28b0f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="28b0f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28b0f-111">Список слушателей onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="28b0f-111">List onSignUpStart listeners</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="28b0f-112">[коллекция authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="28b0f-112">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="28b0f-113">Получите коллекцию ресурсов authenticationListener, поддерживаемую событием onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="28b0f-113">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="28b0f-114">Создание authenticationListener</span><span class="sxs-lookup"><span data-stu-id="28b0f-114">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="28b0f-115">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="28b0f-115">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="28b0f-116">Создайте новый объект authenticationListener для события onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="28b0f-116">Create a new authenticationListener object for the onSignupStart event.</span></span>|

## <a name="properties"></a><span data-ttu-id="28b0f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="28b0f-117">Properties</span></span>

|<span data-ttu-id="28b0f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="28b0f-118">Property</span></span>|<span data-ttu-id="28b0f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="28b0f-119">Type</span></span>|<span data-ttu-id="28b0f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="28b0f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28b0f-121">id</span><span class="sxs-lookup"><span data-stu-id="28b0f-121">id</span></span>|<span data-ttu-id="28b0f-122">String</span><span class="sxs-lookup"><span data-stu-id="28b0f-122">String</span></span>|<span data-ttu-id="28b0f-123">Идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="28b0f-123">The identifier of the policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28b0f-124">Связи</span><span class="sxs-lookup"><span data-stu-id="28b0f-124">Relationships</span></span>

|<span data-ttu-id="28b0f-125">Связь</span><span class="sxs-lookup"><span data-stu-id="28b0f-125">Relationship</span></span>|<span data-ttu-id="28b0f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="28b0f-126">Type</span></span>|<span data-ttu-id="28b0f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="28b0f-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28b0f-128">onSignupStart</span><span class="sxs-lookup"><span data-stu-id="28b0f-128">onSignupStart</span></span>|<span data-ttu-id="28b0f-129">[коллекция authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="28b0f-129">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="28b0f-130">Список применимых действий, которые необходимо принять при регистрации.</span><span class="sxs-lookup"><span data-stu-id="28b0f-130">A list of applicable actions to be taken on sign-up.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28b0f-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28b0f-131">JSON representation</span></span>

<span data-ttu-id="28b0f-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28b0f-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```
