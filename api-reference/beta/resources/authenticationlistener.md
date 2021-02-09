---
title: Тип ресурса authenticationListener
description: Определяет прослушиватель для оценки во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 41114f69bb169922b5594ee5cbbcdb236edfb0d0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159166"
---
# <a name="authenticationlistener-resource-type"></a><span data-ttu-id="93366-103">Тип ресурса authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-103">authenticationListener resource type</span></span>

<span data-ttu-id="93366-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93366-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93366-105">Определяет прослушиватель для оценки события проверки подлинности при проверке подлинности.</span><span class="sxs-lookup"><span data-stu-id="93366-105">Defines a listener to be evaluate when an authentication event happens in an authentication experience.</span></span> <span data-ttu-id="93366-106">AuthenticationListener абстрактный и является базовым классом различных типов прослушивателей, которые можно оценить во время события проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="93366-106">An authenticationListener is abstract and is the base class of the various types of listeners you can evaluate during an authentication event.</span></span> 

<span data-ttu-id="93366-107">Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart..</span><span class="sxs-lookup"><span data-stu-id="93366-107">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event..</span></span> <span data-ttu-id="93366-108">Это связывает приложение с пользовательским потоком, что позволяет [самообслуживить процесс регистрации.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview)</span><span class="sxs-lookup"><span data-stu-id="93366-108">This associates an application with a user flow, therefore enabling a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) process.</span></span> <span data-ttu-id="93366-109">После того как приложение будет связано с потоком пользователей, пользователи, которые будут перейти к этому приложению, смогут инициировать процесс регистрации, который будет подготовка гостевой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="93366-109">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

## <a name="methods"></a><span data-ttu-id="93366-110">Методы</span><span class="sxs-lookup"><span data-stu-id="93366-110">Methods</span></span>

|<span data-ttu-id="93366-111">Метод</span><span class="sxs-lookup"><span data-stu-id="93366-111">Method</span></span>|<span data-ttu-id="93366-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="93366-112">Return type</span></span>|<span data-ttu-id="93366-113">Описание</span><span class="sxs-lookup"><span data-stu-id="93366-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="93366-114">Список onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="93366-114">List onSignUpStart</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="93366-115">[Коллекция authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="93366-115">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="93366-116">Получите коллекцию ресурсов authenticationListener, поддерживаемых событием onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="93366-116">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="93366-117">Создание authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-117">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="93366-118">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-118">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="93366-119">Создайте новый объект authenticationListener для события onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="93366-119">Create a new authenticationListener object for the onSignupStart event.</span></span>|
|[<span data-ttu-id="93366-120">Обновление authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-120">Update authenticationListener</span></span>](../api/authenticationlistener-update.md)|[<span data-ttu-id="93366-121">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-121">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="93366-122">Обновите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="93366-122">Update the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="93366-123">Put authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-123">Put authenticationListener</span></span>](../api/authenticationlistener-put.md)|[<span data-ttu-id="93366-124">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-124">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="93366-125">Замените свойства объекта authenticationListener.</span><span class="sxs-lookup"><span data-stu-id="93366-125">Replace the properties of an authenticationListener object.</span></span>|
|[<span data-ttu-id="93366-126">Get authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-126">Get authenticationListener</span></span>](../api/authenticationlistener-get.md)|[<span data-ttu-id="93366-127">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-127">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="93366-128">Получите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="93366-128">Get the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="93366-129">Удаление authenticationListener</span><span class="sxs-lookup"><span data-stu-id="93366-129">Delete authenticationListener</span></span>](../api/authenticationlistener-delete.md)|<span data-ttu-id="93366-130">Нет</span><span class="sxs-lookup"><span data-stu-id="93366-130">None</span></span>|<span data-ttu-id="93366-131">Удалите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="93366-131">Delete the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|

## <a name="properties"></a><span data-ttu-id="93366-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="93366-132">Properties</span></span>

|<span data-ttu-id="93366-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="93366-133">Property</span></span>|<span data-ttu-id="93366-134">Тип</span><span class="sxs-lookup"><span data-stu-id="93366-134">Type</span></span>|<span data-ttu-id="93366-135">Описание</span><span class="sxs-lookup"><span data-stu-id="93366-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93366-136">id</span><span class="sxs-lookup"><span data-stu-id="93366-136">id</span></span>|<span data-ttu-id="93366-137">String</span><span class="sxs-lookup"><span data-stu-id="93366-137">String</span></span>|<span data-ttu-id="93366-138">Идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="93366-138">The identifier of the action.</span></span>|
|<span data-ttu-id="93366-139">priority</span><span class="sxs-lookup"><span data-stu-id="93366-139">priority</span></span>|<span data-ttu-id="93366-140">Int32</span><span class="sxs-lookup"><span data-stu-id="93366-140">Int32</span></span>|<span data-ttu-id="93366-141">Приоритет прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="93366-141">The priority of the listener.</span></span> <span data-ttu-id="93366-142">Определяет порядок оценки, если событие имеет несколько прослушивателей.</span><span class="sxs-lookup"><span data-stu-id="93366-142">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="93366-143">Приоритет оценивается от низкого до высокого.</span><span class="sxs-lookup"><span data-stu-id="93366-143">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="93366-144">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="93366-144">sourceFilter</span></span>|[<span data-ttu-id="93366-145">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="93366-145">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="93366-146">Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="93366-146">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="93366-147">В настоящее время это ограничение ограничено оценками, основанными на приложении, в которое пользователь проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="93366-147">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93366-148">Связи</span><span class="sxs-lookup"><span data-stu-id="93366-148">Relationships</span></span>

<span data-ttu-id="93366-149">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="93366-149">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93366-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="93366-150">JSON representation</span></span>

<span data-ttu-id="93366-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93366-151">The following is a JSON representation of the resource.</span></span>
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
