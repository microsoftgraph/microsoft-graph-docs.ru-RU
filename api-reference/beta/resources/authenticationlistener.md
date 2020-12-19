---
title: Тип ресурса authenticationListener
description: Определяет прослушиватель для оценки во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d89d7660fc2580b8fad185633b6b819df1a41aaf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720353"
---
# <a name="authenticationlistener-resource-type"></a><span data-ttu-id="f7b79-103">Тип ресурса authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-103">authenticationListener resource type</span></span>

<span data-ttu-id="f7b79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7b79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b79-105">Определяет прослушиватель, который будет оцениваться при событии проверки подлинности при проверке подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7b79-105">Defines a listener to be evaluate when an authentication event happens in an authentication experience.</span></span> <span data-ttu-id="f7b79-106">AuthenticationListener абстрактный и является базовым классом различных типов прослушивателей, которые можно оценить во время события проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7b79-106">An authenticationListener is abstract and is the base class of the various types of listeners you can evaluate during an authentication event.</span></span> 

<span data-ttu-id="f7b79-107">Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart..</span><span class="sxs-lookup"><span data-stu-id="f7b79-107">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event..</span></span> <span data-ttu-id="f7b79-108">Это связывает приложение с пользовательским потоком, что позволяет самообслуживить [процесс регистрации.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview)</span><span class="sxs-lookup"><span data-stu-id="f7b79-108">This associates an application with a user flow, therefore enabling a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) process.</span></span> <span data-ttu-id="f7b79-109">После того как приложение будет связано с потоком пользователей, пользователи, которые будут перейти к этому приложению, смогут инициировать процесс регистрации, который подавит гостевую учетную запись.</span><span class="sxs-lookup"><span data-stu-id="f7b79-109">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

## <a name="methods"></a><span data-ttu-id="f7b79-110">Методы</span><span class="sxs-lookup"><span data-stu-id="f7b79-110">Methods</span></span>

|<span data-ttu-id="f7b79-111">Метод</span><span class="sxs-lookup"><span data-stu-id="f7b79-111">Method</span></span>|<span data-ttu-id="f7b79-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="f7b79-112">Return type</span></span>|<span data-ttu-id="f7b79-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f7b79-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7b79-114">Список onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="f7b79-114">List onSignUpStart</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="f7b79-115">[Коллекция authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="f7b79-115">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="f7b79-116">Получите коллекцию ресурсов authenticationListener, поддерживаемых событием onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="f7b79-116">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="f7b79-117">Создание authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-117">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="f7b79-118">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-118">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="f7b79-119">Создайте новый объект authenticationListener для события onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="f7b79-119">Create a new authenticationListener object for the onSignupStart event.</span></span>|
|[<span data-ttu-id="f7b79-120">Обновление authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-120">Update authenticationListener</span></span>](../api/authenticationlistener-update.md)|[<span data-ttu-id="f7b79-121">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-121">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="f7b79-122">Обновите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7b79-122">Update the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="f7b79-123">Put authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-123">Put authenticationListener</span></span>](../api/authenticationlistener-put.md)|[<span data-ttu-id="f7b79-124">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-124">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="f7b79-125">Замените свойства объекта authenticationListener.</span><span class="sxs-lookup"><span data-stu-id="f7b79-125">Replace the properties of an authenticationListener object.</span></span>|
|[<span data-ttu-id="f7b79-126">Get authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-126">Get authenticationListener</span></span>](../api/authenticationlistener-get.md)|[<span data-ttu-id="f7b79-127">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-127">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="f7b79-128">Получите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7b79-128">Get the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="f7b79-129">Удаление authenticationListener</span><span class="sxs-lookup"><span data-stu-id="f7b79-129">Delete authenticationListener</span></span>](../api/authenticationlistener-delete.md)|<span data-ttu-id="f7b79-130">Нет</span><span class="sxs-lookup"><span data-stu-id="f7b79-130">None</span></span>|<span data-ttu-id="f7b79-131">Удалите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7b79-131">Delete the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7b79-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7b79-132">Properties</span></span>

|<span data-ttu-id="f7b79-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7b79-133">Property</span></span>|<span data-ttu-id="f7b79-134">Тип</span><span class="sxs-lookup"><span data-stu-id="f7b79-134">Type</span></span>|<span data-ttu-id="f7b79-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f7b79-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7b79-136">id</span><span class="sxs-lookup"><span data-stu-id="f7b79-136">id</span></span>|<span data-ttu-id="f7b79-137">String</span><span class="sxs-lookup"><span data-stu-id="f7b79-137">String</span></span>|<span data-ttu-id="f7b79-138">Идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="f7b79-138">The identifier of the action.</span></span>|
|<span data-ttu-id="f7b79-139">priority</span><span class="sxs-lookup"><span data-stu-id="f7b79-139">priority</span></span>|<span data-ttu-id="f7b79-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f7b79-140">Int32</span></span>|<span data-ttu-id="f7b79-141">Приоритет прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="f7b79-141">The priority of the listener.</span></span> <span data-ttu-id="f7b79-142">Определяет порядок оценки, если событие имеет несколько прослушивателей.</span><span class="sxs-lookup"><span data-stu-id="f7b79-142">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="f7b79-143">Приоритет оценивается от низкого до высокого.</span><span class="sxs-lookup"><span data-stu-id="f7b79-143">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="f7b79-144">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="f7b79-144">sourceFilter</span></span>|[<span data-ttu-id="f7b79-145">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="f7b79-145">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="f7b79-146">Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="f7b79-146">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="f7b79-147">В настоящее время это ограничение ограничено оценками, основанными на приложении, в которое пользователь проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7b79-147">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7b79-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="f7b79-148">Relationships</span></span>

<span data-ttu-id="f7b79-149">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f7b79-149">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7b79-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f7b79-150">JSON representation</span></span>

<span data-ttu-id="f7b79-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7b79-151">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "baseType": "",
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
