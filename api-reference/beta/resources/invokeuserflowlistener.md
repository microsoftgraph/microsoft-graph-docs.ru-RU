---
title: тип ресурса invokeUserFlowListener
description: Прослушиватель, используемый для вызова потока пользователей во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 89f990ab4692ec7fd4d6ce3b94ee4c4d4846c6c4
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547213"
---
# <a name="invokeuserflowlistener-resource-type"></a><span data-ttu-id="58b41-103">тип ресурса invokeUserFlowListener</span><span class="sxs-lookup"><span data-stu-id="58b41-103">invokeUserFlowListener resource type</span></span>

<span data-ttu-id="58b41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58b41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58b41-105">Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="58b41-105">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event.</span></span> <span data-ttu-id="58b41-106">Это связывает приложение с потоком пользователей, который позволяет самостоятельной регистрации внешних удостоверений [для](/azure/active-directory/external-identities/self-service-sign-up-overview) приложения.</span><span class="sxs-lookup"><span data-stu-id="58b41-106">This associates an application with a user flow, which enables [external identities self-service sign up](/azure/active-directory/external-identities/self-service-sign-up-overview) for the application.</span></span> <span data-ttu-id="58b41-107">После того как приложение связано с потоком пользователей, пользователи, которые идут в это приложение, смогут инициировать поток регистрации, который содержит учетную запись для гостей.</span><span class="sxs-lookup"><span data-stu-id="58b41-107">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

<span data-ttu-id="58b41-108">Наследуется от абстрактного базового типа [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="58b41-108">Inherits from the abstract base type [authenticationListener](../resources/authenticationlistener.md).</span></span>

## <a name="properties"></a><span data-ttu-id="58b41-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="58b41-109">Properties</span></span>

|<span data-ttu-id="58b41-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="58b41-110">Property</span></span>|<span data-ttu-id="58b41-111">Тип</span><span class="sxs-lookup"><span data-stu-id="58b41-111">Type</span></span>|<span data-ttu-id="58b41-112">Описание</span><span class="sxs-lookup"><span data-stu-id="58b41-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b41-113">id</span><span class="sxs-lookup"><span data-stu-id="58b41-113">id</span></span>|<span data-ttu-id="58b41-114">String</span><span class="sxs-lookup"><span data-stu-id="58b41-114">String</span></span>|<span data-ttu-id="58b41-115">Идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="58b41-115">The identifier of the action.</span></span> <span data-ttu-id="58b41-116">Наследуется [от authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="58b41-116">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="58b41-117">priority</span><span class="sxs-lookup"><span data-stu-id="58b41-117">priority</span></span>|<span data-ttu-id="58b41-118">Int32</span><span class="sxs-lookup"><span data-stu-id="58b41-118">Int32</span></span>|<span data-ttu-id="58b41-119">Приоритет действия, используемого для определения одного из нескольких применимых действий.</span><span class="sxs-lookup"><span data-stu-id="58b41-119">The priority of the action that is used to determine one out of multiple applicable actions.</span></span> <span data-ttu-id="58b41-120">Наследуется [от authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="58b41-120">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="58b41-121">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="58b41-121">sourceFilter</span></span>|[<span data-ttu-id="58b41-122">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="58b41-122">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="58b41-123">Фильтр на основе источника проверки подлинности, который используется для определения того, выполняется ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="58b41-123">Filter based on the source of the authentication that is used to determine whether the listener is executed.</span></span> <span data-ttu-id="58b41-124">Наследуется [от authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="58b41-124">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="58b41-125">Связи</span><span class="sxs-lookup"><span data-stu-id="58b41-125">Relationships</span></span>

|<span data-ttu-id="58b41-126">Связь</span><span class="sxs-lookup"><span data-stu-id="58b41-126">Relationship</span></span>|<span data-ttu-id="58b41-127">Тип</span><span class="sxs-lookup"><span data-stu-id="58b41-127">Type</span></span>|<span data-ttu-id="58b41-128">Описание</span><span class="sxs-lookup"><span data-stu-id="58b41-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b41-129">userFlow</span><span class="sxs-lookup"><span data-stu-id="58b41-129">userFlow</span></span>|[<span data-ttu-id="58b41-130">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="58b41-130">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="58b41-131">Поток пользователей, вызываемый при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="58b41-131">The user flow that is invoked when this action executes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58b41-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58b41-132">JSON representation</span></span>

<span data-ttu-id="58b41-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58b41-133">The following is a JSON representation of the resource.</span></span>
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
