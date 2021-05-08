---
title: Тип ресурса authenticationFlowsPolicy
description: 'Представляет конфигурацию политики для интерфейса самостоятельной регистрации на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 369ad06f9d653054c6b165b0ebc2daa3e8d402c6
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231258"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="c9ee8-103">Тип ресурса authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="c9ee8-103">authenticationFlowsPolicy resource type</span></span>

<span data-ttu-id="c9ee8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9ee8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9ee8-105">Представляет [конфигурацию политики для интерфейса самостоятельной регистрации](../resources/selfservicesignupauthenticationflowconfiguration.md) на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="c9ee8-106">Содержит такие сведения, как идентификатор, отображаемое имя и описание, а также указывает, включена ли для политики самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-106">It contains information, such as the identifier, display name, and description, and indicates whether self-service sign-up is enabled for the policy.</span></span>

## <a name="methods"></a><span data-ttu-id="c9ee8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c9ee8-107">Methods</span></span>

| <span data-ttu-id="c9ee8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c9ee8-108">Method</span></span>       | <span data-ttu-id="c9ee8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c9ee8-109">Return Type</span></span>  |<span data-ttu-id="c9ee8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c9ee8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9ee8-111">Получение политики потоков проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="c9ee8-111">Get authentication flows policy</span></span>](../api/authenticationflowspolicy-get.md)|<span data-ttu-id="c9ee8-112">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="c9ee8-112">authenticationFlowsPolicy</span></span>|<span data-ttu-id="c9ee8-113">Получение конфигурации политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-113">Get the authentication flows policy configuration.</span></span>|
|[<span data-ttu-id="c9ee8-114">Обновление политики потоков проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="c9ee8-114">Update authentication flows policy</span></span>](../api/authenticationflowspolicy-update.md)|<span data-ttu-id="c9ee8-115">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="c9ee8-115">authenticationFlowsPolicy</span></span>|<span data-ttu-id="c9ee8-116">Обновление конфигурации политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-116">Update the authentication flows policy configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9ee8-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9ee8-117">Properties</span></span>

|<span data-ttu-id="c9ee8-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9ee8-118">Property</span></span>|<span data-ttu-id="c9ee8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c9ee8-119">Type</span></span>|<span data-ttu-id="c9ee8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c9ee8-120">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="c9ee8-121">id</span><span class="sxs-lookup"><span data-stu-id="c9ee8-121">id</span></span>|<span data-ttu-id="c9ee8-122">Строка</span><span class="sxs-lookup"><span data-stu-id="c9ee8-122">String</span></span>| <span data-ttu-id="c9ee8-123">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-123">Inherited property.</span></span> <span data-ttu-id="c9ee8-124">Идентификатор политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-124">The identifier of the authentication flows policy.</span></span> <span data-ttu-id="c9ee8-125">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-125">Optional.</span></span> <span data-ttu-id="c9ee8-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-126">Read-only.</span></span>
|<span data-ttu-id="c9ee8-127">displayName</span><span class="sxs-lookup"><span data-stu-id="c9ee8-127">displayName</span></span>|<span data-ttu-id="c9ee8-128">Строка</span><span class="sxs-lookup"><span data-stu-id="c9ee8-128">String</span></span>| <span data-ttu-id="c9ee8-129">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-129">Inherited property.</span></span> <span data-ttu-id="c9ee8-130">Понятное для пользователя имя политики.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-130">The human-readable name of the policy.</span></span> <span data-ttu-id="c9ee8-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-131">Optional.</span></span> <span data-ttu-id="c9ee8-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-132">Read-only.</span></span>|
|<span data-ttu-id="c9ee8-133">description</span><span class="sxs-lookup"><span data-stu-id="c9ee8-133">description</span></span>|<span data-ttu-id="c9ee8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c9ee8-134">String</span></span>|<span data-ttu-id="c9ee8-135">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-135">Inherited property.</span></span> <span data-ttu-id="c9ee8-136">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-136">A description of the policy.</span></span> <span data-ttu-id="c9ee8-137">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-137">Optional.</span></span> <span data-ttu-id="c9ee8-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-138">Read-only.</span></span>|
|<span data-ttu-id="c9ee8-139">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="c9ee8-139">selfServiceSignUp</span></span>|[<span data-ttu-id="c9ee8-140">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9ee8-140">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="c9ee8-141">Содержит параметры [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md), описывающие, включена ли самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-141">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="c9ee8-142">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-142">Optional.</span></span> <span data-ttu-id="c9ee8-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-143">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c9ee8-144">Связи</span><span class="sxs-lookup"><span data-stu-id="c9ee8-144">Relationships</span></span>

<span data-ttu-id="c9ee8-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9ee8-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c9ee8-146">JSON representation</span></span>

<span data-ttu-id="c9ee8-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9ee8-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "openType": false
}
-->

``` json
{
   "id":"String (identifier)",
   "displayName":"String",
   "description":"String",
   "selfServiceSignUp":{
      "@odata.type":"#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
   }
}
```
