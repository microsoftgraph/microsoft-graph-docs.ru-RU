---
title: Тип ресурса authenticationFlowsPolicy
description: 'Представляет конфигурацию политики для интерфейса самостоятельной регистрации на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ea0ca54c4be4e80043ac9560d2b8dd3744584aa9
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883056"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="60af1-103">Тип ресурса authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="60af1-103">authenticationFlowsPolicy resource type</span></span>

<span data-ttu-id="60af1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60af1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60af1-105">Представляет [конфигурацию политики для интерфейса самостоятельной регистрации](../resources/selfservicesignupauthenticationflowconfiguration.md) на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации.</span><span class="sxs-lookup"><span data-stu-id="60af1-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="60af1-106">Содержит такие сведения, как идентификатор, отображаемое имя и описание, а также указывает, включена ли для политики самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="60af1-106">It contains information, such as the identifier, display name, and description, and indicates whether self-service sign-up is enabled for the policy.</span></span>

## <a name="methods"></a><span data-ttu-id="60af1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="60af1-107">Methods</span></span>

| <span data-ttu-id="60af1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="60af1-108">Method</span></span>       | <span data-ttu-id="60af1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60af1-109">Return Type</span></span>  |<span data-ttu-id="60af1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="60af1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60af1-111">Получение политики потоков проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="60af1-111">Get authentication flows policy</span></span>](../api/authenticationflowspolicy-get.md)|<span data-ttu-id="60af1-112">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="60af1-112">authenticationFlowsPolicy</span></span>|<span data-ttu-id="60af1-113">Получение конфигурации политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="60af1-113">Get the authentication flows policy configuration.</span></span>|
|[<span data-ttu-id="60af1-114">Обновление политики потоков проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="60af1-114">Update authentication flows policy</span></span>](../api/authenticationflowspolicy-update.md)|<span data-ttu-id="60af1-115">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="60af1-115">authenticationFlowsPolicy</span></span>|<span data-ttu-id="60af1-116">Обновление конфигурации политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="60af1-116">Update the authentication flows policy configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="60af1-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="60af1-117">Properties</span></span>

|<span data-ttu-id="60af1-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="60af1-118">Property</span></span>|<span data-ttu-id="60af1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="60af1-119">Type</span></span>|<span data-ttu-id="60af1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="60af1-120">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="60af1-121">id</span><span class="sxs-lookup"><span data-stu-id="60af1-121">id</span></span>|<span data-ttu-id="60af1-122">Строка</span><span class="sxs-lookup"><span data-stu-id="60af1-122">String</span></span>| <span data-ttu-id="60af1-123">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="60af1-123">Inherited property.</span></span> <span data-ttu-id="60af1-124">Идентификатор политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="60af1-124">The identifier of the authentication flows policy.</span></span> <span data-ttu-id="60af1-125">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="60af1-125">Optional.</span></span> <span data-ttu-id="60af1-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60af1-126">Read-only.</span></span>
|<span data-ttu-id="60af1-127">displayName</span><span class="sxs-lookup"><span data-stu-id="60af1-127">displayName</span></span>|<span data-ttu-id="60af1-128">Строка</span><span class="sxs-lookup"><span data-stu-id="60af1-128">String</span></span>| <span data-ttu-id="60af1-129">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="60af1-129">Inherited property.</span></span> <span data-ttu-id="60af1-130">Понятное для пользователя имя политики.</span><span class="sxs-lookup"><span data-stu-id="60af1-130">The human-readable name of the policy.</span></span> <span data-ttu-id="60af1-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="60af1-131">Optional.</span></span> <span data-ttu-id="60af1-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60af1-132">Read-only.</span></span>|
|<span data-ttu-id="60af1-133">description</span><span class="sxs-lookup"><span data-stu-id="60af1-133">description</span></span>|<span data-ttu-id="60af1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="60af1-134">String</span></span>|<span data-ttu-id="60af1-135">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="60af1-135">Inherited property.</span></span> <span data-ttu-id="60af1-136">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="60af1-136">A description of the policy.</span></span> <span data-ttu-id="60af1-137">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="60af1-137">Optional.</span></span> <span data-ttu-id="60af1-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60af1-138">Read-only.</span></span>|
|<span data-ttu-id="60af1-139">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="60af1-139">selfServiceSignUp</span></span>|[<span data-ttu-id="60af1-140">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="60af1-140">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="60af1-141">Содержит параметры [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md), описывающие, включена ли самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="60af1-141">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="60af1-142">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="60af1-142">Optional.</span></span> <span data-ttu-id="60af1-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60af1-143">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="60af1-144">Связи</span><span class="sxs-lookup"><span data-stu-id="60af1-144">Relationships</span></span>

<span data-ttu-id="60af1-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="60af1-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60af1-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="60af1-146">JSON representation</span></span>

<span data-ttu-id="60af1-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60af1-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "selfServiceSignUp": {
    "@odata.type": "#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
  },
}
```
