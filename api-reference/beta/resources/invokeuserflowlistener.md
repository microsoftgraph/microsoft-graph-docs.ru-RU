---
title: тип ресурса invokeUserFlowListener
description: Прослушиватель, используемый для вызова потока пользователей во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7eee91460c623be982cb316edae1c3c2f0734b07
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442994"
---
# <a name="invokeuserflowlistener-resource-type"></a><span data-ttu-id="77882-103">тип ресурса invokeUserFlowListener</span><span class="sxs-lookup"><span data-stu-id="77882-103">invokeUserFlowListener resource type</span></span>

<span data-ttu-id="77882-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77882-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77882-105">Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="77882-105">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event.</span></span> <span data-ttu-id="77882-106">Это связывает приложение с потоком пользователей, который позволяет самостоятельной регистрации внешних удостоверений [для](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) приложения.</span><span class="sxs-lookup"><span data-stu-id="77882-106">This associates an application with a user flow, which enables [external identities self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) for the application.</span></span> <span data-ttu-id="77882-107">После того как приложение связано с потоком пользователей, пользователи, которые идут в это приложение, смогут инициировать поток регистрации, который содержит учетную запись для гостей.</span><span class="sxs-lookup"><span data-stu-id="77882-107">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

<span data-ttu-id="77882-108">Наследуется от абстрактного базового типа [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="77882-108">Inherits from the abstract base type [authenticationListener](../resources/authenticationlistener.md).</span></span>

## <a name="properties"></a><span data-ttu-id="77882-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="77882-109">Properties</span></span>

|<span data-ttu-id="77882-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="77882-110">Property</span></span>|<span data-ttu-id="77882-111">Тип</span><span class="sxs-lookup"><span data-stu-id="77882-111">Type</span></span>|<span data-ttu-id="77882-112">Описание</span><span class="sxs-lookup"><span data-stu-id="77882-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77882-113">id</span><span class="sxs-lookup"><span data-stu-id="77882-113">id</span></span>|<span data-ttu-id="77882-114">String</span><span class="sxs-lookup"><span data-stu-id="77882-114">String</span></span>|<span data-ttu-id="77882-115">Идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="77882-115">The identifier of the action.</span></span> <span data-ttu-id="77882-116">Наследуется [от authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="77882-116">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="77882-117">priority</span><span class="sxs-lookup"><span data-stu-id="77882-117">priority</span></span>|<span data-ttu-id="77882-118">Int32</span><span class="sxs-lookup"><span data-stu-id="77882-118">Int32</span></span>|<span data-ttu-id="77882-119">Приоритет действия, используемого для определения одного из нескольких применимых действий.</span><span class="sxs-lookup"><span data-stu-id="77882-119">The priority of the action that is used to determine one out of multiple applicable actions.</span></span> <span data-ttu-id="77882-120">Наследуется [от authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="77882-120">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="77882-121">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="77882-121">sourceFilter</span></span>|[<span data-ttu-id="77882-122">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="77882-122">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="77882-123">Фильтр на основе источника проверки подлинности, который используется для определения того, выполняется ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="77882-123">Filter based on the source of the authentication that is used to determine whether the listener is executed.</span></span> <span data-ttu-id="77882-124">Наследуется [от authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="77882-124">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="77882-125">Связи</span><span class="sxs-lookup"><span data-stu-id="77882-125">Relationships</span></span>

|<span data-ttu-id="77882-126">Связь</span><span class="sxs-lookup"><span data-stu-id="77882-126">Relationship</span></span>|<span data-ttu-id="77882-127">Тип</span><span class="sxs-lookup"><span data-stu-id="77882-127">Type</span></span>|<span data-ttu-id="77882-128">Описание</span><span class="sxs-lookup"><span data-stu-id="77882-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77882-129">userFlow</span><span class="sxs-lookup"><span data-stu-id="77882-129">userFlow</span></span>|[<span data-ttu-id="77882-130">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="77882-130">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="77882-131">Поток пользователей, вызываемый при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="77882-131">The user flow that is invoked when this action executes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77882-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77882-132">JSON representation</span></span>

<span data-ttu-id="77882-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77882-133">The following is a JSON representation of the resource.</span></span>
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
