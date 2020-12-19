---
title: Тип ресурса invokeUserFlowListener
description: Прослушиватель, используемый для вызова пользовательского потока во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ca1c61d830a2ff98f2d72839129d75cc6287c36
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720437"
---
# <a name="invokeuserflowlistener-resource-type"></a><span data-ttu-id="1224c-103">Тип ресурса invokeUserFlowListener</span><span class="sxs-lookup"><span data-stu-id="1224c-103">invokeUserFlowListener resource type</span></span>

<span data-ttu-id="1224c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1224c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1224c-105">Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="1224c-105">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event.</span></span> <span data-ttu-id="1224c-106">Это связывает приложение с пользовательским потоком, что позволяет внешним удостоверениям самостоятельно зарегистрироваться [в](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) приложении.</span><span class="sxs-lookup"><span data-stu-id="1224c-106">This associates an application with a user flow, which enables [external identities self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) for the application.</span></span> <span data-ttu-id="1224c-107">После того как приложение будет связано с потоком пользователей, пользователи, которые будут перейти к этому приложению, смогут инициировать процесс регистрации, который будет подготовка гостевой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="1224c-107">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

<span data-ttu-id="1224c-108">Наследуется от абстрактного базового типа [authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="1224c-108">Inherits from the abstract base type [authenticationListener](../resources/authenticationlistener.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1224c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1224c-109">Properties</span></span>

|<span data-ttu-id="1224c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1224c-110">Property</span></span>|<span data-ttu-id="1224c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1224c-111">Type</span></span>|<span data-ttu-id="1224c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1224c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1224c-113">id</span><span class="sxs-lookup"><span data-stu-id="1224c-113">id</span></span>|<span data-ttu-id="1224c-114">String</span><span class="sxs-lookup"><span data-stu-id="1224c-114">String</span></span>|<span data-ttu-id="1224c-115">Идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="1224c-115">The identifier of the action.</span></span> <span data-ttu-id="1224c-116">Наследуется [от authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="1224c-116">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="1224c-117">priority</span><span class="sxs-lookup"><span data-stu-id="1224c-117">priority</span></span>|<span data-ttu-id="1224c-118">Int32</span><span class="sxs-lookup"><span data-stu-id="1224c-118">Int32</span></span>|<span data-ttu-id="1224c-119">Приоритет действия, используемого для определения одного из нескольких применимых действий.</span><span class="sxs-lookup"><span data-stu-id="1224c-119">The priority of the action that is used to determine one out of multiple applicable actions.</span></span> <span data-ttu-id="1224c-120">Наследуется [от authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="1224c-120">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="1224c-121">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="1224c-121">sourceFilter</span></span>|[<span data-ttu-id="1224c-122">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="1224c-122">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="1224c-123">Фильтрация на основе источника проверки подлинности, используемого для определения того, выполняется ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="1224c-123">Filter based on the source of the authentication that is used to determine whether the listener is executed.</span></span> <span data-ttu-id="1224c-124">Наследуется [от authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="1224c-124">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1224c-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="1224c-125">Relationships</span></span>

|<span data-ttu-id="1224c-126">Связь</span><span class="sxs-lookup"><span data-stu-id="1224c-126">Relationship</span></span>|<span data-ttu-id="1224c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1224c-127">Type</span></span>|<span data-ttu-id="1224c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1224c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1224c-129">userFlow</span><span class="sxs-lookup"><span data-stu-id="1224c-129">userFlow</span></span>|[<span data-ttu-id="1224c-130">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="1224c-130">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="1224c-131">Пользовательский поток, который вызывается при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="1224c-131">The user flow that is invoked when this action executes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1224c-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1224c-132">JSON representation</span></span>

<span data-ttu-id="1224c-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1224c-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.invokeUserFlowListener",
  "baseType": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  },
  "userFlow": {
    "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
  }
}
```
