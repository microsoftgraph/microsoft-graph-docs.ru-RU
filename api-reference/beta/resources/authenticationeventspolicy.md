---
title: Тип ресурса authenticationEventsPolicy
description: События проверки подлинности используются для вызова пользовательских потоков в определенных точках потока проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4fe50176ebf49d79adc1db55c657bcf7fed8f096
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159955"
---
# <a name="authenticationeventspolicy-resource-type"></a><span data-ttu-id="efb8a-103">Тип ресурса authenticationEventsPolicy</span><span class="sxs-lookup"><span data-stu-id="efb8a-103">authenticationEventsPolicy resource type</span></span>

<span data-ttu-id="efb8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efb8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efb8a-105">Ресурс, определяющий события в средстве проверки подлинности, при этом каждое событие дополнительно определяет доступные типы прослушивателей, которые можно создать для события.</span><span class="sxs-lookup"><span data-stu-id="efb8a-105">A resource that specifies the events in the authentication experience, with each event further defining the available types of listeners that can be created for the event.</span></span> <span data-ttu-id="efb8a-106">События являются неотъемлемой частью проверки подлинности; Этот ресурс не настраивается пользователем.</span><span class="sxs-lookup"><span data-stu-id="efb8a-106">Events are inherent to the authentication experience; this resource is not user configurable.</span></span>

## <a name="methods"></a><span data-ttu-id="efb8a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="efb8a-107">Methods</span></span>

|<span data-ttu-id="efb8a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="efb8a-108">Method</span></span>|<span data-ttu-id="efb8a-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="efb8a-109">Return type</span></span>|<span data-ttu-id="efb8a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="efb8a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="efb8a-111">Список прослушивателей onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="efb8a-111">List onSignUpStart listeners</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="efb8a-112">[Коллекция authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="efb8a-112">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="efb8a-113">Получите коллекцию ресурсов authenticationListener, поддерживаемых событием onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="efb8a-113">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="efb8a-114">Создание authenticationListener</span><span class="sxs-lookup"><span data-stu-id="efb8a-114">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="efb8a-115">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="efb8a-115">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="efb8a-116">Создайте новый объект authenticationListener для события onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="efb8a-116">Create a new authenticationListener object for the onSignupStart event.</span></span>|

## <a name="properties"></a><span data-ttu-id="efb8a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="efb8a-117">Properties</span></span>

|<span data-ttu-id="efb8a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="efb8a-118">Property</span></span>|<span data-ttu-id="efb8a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="efb8a-119">Type</span></span>|<span data-ttu-id="efb8a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="efb8a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb8a-121">id</span><span class="sxs-lookup"><span data-stu-id="efb8a-121">id</span></span>|<span data-ttu-id="efb8a-122">String</span><span class="sxs-lookup"><span data-stu-id="efb8a-122">String</span></span>|<span data-ttu-id="efb8a-123">Идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="efb8a-123">The identifier of the policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efb8a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="efb8a-124">Relationships</span></span>

|<span data-ttu-id="efb8a-125">Связь</span><span class="sxs-lookup"><span data-stu-id="efb8a-125">Relationship</span></span>|<span data-ttu-id="efb8a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="efb8a-126">Type</span></span>|<span data-ttu-id="efb8a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="efb8a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb8a-128">onSignupStart</span><span class="sxs-lookup"><span data-stu-id="efb8a-128">onSignupStart</span></span>|<span data-ttu-id="efb8a-129">[Коллекция authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="efb8a-129">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="efb8a-130">Список применимых действий, которые необходимо принять при регистрации.</span><span class="sxs-lookup"><span data-stu-id="efb8a-130">A list of applicable actions to be taken on sign-up.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efb8a-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efb8a-131">JSON representation</span></span>

<span data-ttu-id="efb8a-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efb8a-132">The following is a JSON representation of the resource.</span></span>
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
