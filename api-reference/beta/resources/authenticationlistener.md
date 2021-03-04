---
title: тип ресурса authenticationListener
description: Определяет слушателя для оценки во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a7feeabaa9caf0246a53aded7ac1c15236fdf8af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433189"
---
# <a name="authenticationlistener-resource-type"></a><span data-ttu-id="0ce81-103">тип ресурса authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-103">authenticationListener resource type</span></span>

<span data-ttu-id="0ce81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ce81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ce81-105">Определяет слушателя, который должен оценивать, когда событие проверки подлинности происходит при проверке подлинности.</span><span class="sxs-lookup"><span data-stu-id="0ce81-105">Defines a listener to be evaluate when an authentication event happens in an authentication experience.</span></span> <span data-ttu-id="0ce81-106">АутентификацияListener абстрактна и является базовым классом различных типов слушателей, которые можно оценить во время события проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0ce81-106">An authenticationListener is abstract and is the base class of the various types of listeners you can evaluate during an authentication event.</span></span> 

<span data-ttu-id="0ce81-107">Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart..</span><span class="sxs-lookup"><span data-stu-id="0ce81-107">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event..</span></span> <span data-ttu-id="0ce81-108">Это связывает приложение с потоком пользователей, что позволяет самообслуживывать [процесс регистрации.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview)</span><span class="sxs-lookup"><span data-stu-id="0ce81-108">This associates an application with a user flow, therefore enabling a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) process.</span></span> <span data-ttu-id="0ce81-109">После того как приложение связано с потоком пользователей, пользователи, которые идут в это приложение, смогут инициировать поток регистрации, который содержит учетную запись для гостей.</span><span class="sxs-lookup"><span data-stu-id="0ce81-109">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

## <a name="methods"></a><span data-ttu-id="0ce81-110">Методы</span><span class="sxs-lookup"><span data-stu-id="0ce81-110">Methods</span></span>

|<span data-ttu-id="0ce81-111">Метод</span><span class="sxs-lookup"><span data-stu-id="0ce81-111">Method</span></span>|<span data-ttu-id="0ce81-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="0ce81-112">Return type</span></span>|<span data-ttu-id="0ce81-113">Описание</span><span class="sxs-lookup"><span data-stu-id="0ce81-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0ce81-114">Список onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="0ce81-114">List onSignUpStart</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="0ce81-115">[коллекция authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="0ce81-115">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="0ce81-116">Получите коллекцию ресурсов authenticationListener, поддерживаемую событием onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="0ce81-116">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="0ce81-117">Создание authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-117">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="0ce81-118">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-118">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="0ce81-119">Создайте новый объект authenticationListener для события onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="0ce81-119">Create a new authenticationListener object for the onSignupStart event.</span></span>|
|[<span data-ttu-id="0ce81-120">Обновление проверки подлинностиListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-120">Update authenticationListener</span></span>](../api/authenticationlistener-update.md)|[<span data-ttu-id="0ce81-121">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-121">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="0ce81-122">Обновление указанного слушателя, определенного для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0ce81-122">Update the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="0ce81-123">Put authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-123">Put authenticationListener</span></span>](../api/authenticationlistener-put.md)|[<span data-ttu-id="0ce81-124">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-124">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="0ce81-125">Замените свойства объекта authenticationListener.</span><span class="sxs-lookup"><span data-stu-id="0ce81-125">Replace the properties of an authenticationListener object.</span></span>|
|[<span data-ttu-id="0ce81-126">Получить проверку подлинностиListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-126">Get authenticationListener</span></span>](../api/authenticationlistener-get.md)|[<span data-ttu-id="0ce81-127">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-127">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="0ce81-128">Получите указанный слушатель, определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0ce81-128">Get the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="0ce81-129">Удаление проверки подлинностиListener</span><span class="sxs-lookup"><span data-stu-id="0ce81-129">Delete authenticationListener</span></span>](../api/authenticationlistener-delete.md)|<span data-ttu-id="0ce81-130">Нет</span><span class="sxs-lookup"><span data-stu-id="0ce81-130">None</span></span>|<span data-ttu-id="0ce81-131">Удаление указанного слушателя, определенного для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0ce81-131">Delete the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ce81-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ce81-132">Properties</span></span>

|<span data-ttu-id="0ce81-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ce81-133">Property</span></span>|<span data-ttu-id="0ce81-134">Тип</span><span class="sxs-lookup"><span data-stu-id="0ce81-134">Type</span></span>|<span data-ttu-id="0ce81-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0ce81-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ce81-136">id</span><span class="sxs-lookup"><span data-stu-id="0ce81-136">id</span></span>|<span data-ttu-id="0ce81-137">String</span><span class="sxs-lookup"><span data-stu-id="0ce81-137">String</span></span>|<span data-ttu-id="0ce81-138">Идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="0ce81-138">The identifier of the action.</span></span>|
|<span data-ttu-id="0ce81-139">priority</span><span class="sxs-lookup"><span data-stu-id="0ce81-139">priority</span></span>|<span data-ttu-id="0ce81-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0ce81-140">Int32</span></span>|<span data-ttu-id="0ce81-141">Приоритет слушателя.</span><span class="sxs-lookup"><span data-stu-id="0ce81-141">The priority of the listener.</span></span> <span data-ttu-id="0ce81-142">Определяет порядок оценки, когда в событии имеется несколько слушателей.</span><span class="sxs-lookup"><span data-stu-id="0ce81-142">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="0ce81-143">Приоритет оценивается от низкого до высокого.</span><span class="sxs-lookup"><span data-stu-id="0ce81-143">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="0ce81-144">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="0ce81-144">sourceFilter</span></span>|[<span data-ttu-id="0ce81-145">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="0ce81-145">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="0ce81-146">Фильтр на основе источника проверки подлинности, который используется для определения оценки прослушиваемого.</span><span class="sxs-lookup"><span data-stu-id="0ce81-146">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="0ce81-147">В настоящее время это ограничивается оценками на основе приложения, в которое пользователь проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="0ce81-147">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ce81-148">Связи</span><span class="sxs-lookup"><span data-stu-id="0ce81-148">Relationships</span></span>

<span data-ttu-id="0ce81-149">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0ce81-149">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ce81-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0ce81-150">JSON representation</span></span>

<span data-ttu-id="0ce81-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ce81-151">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  }
}
```
