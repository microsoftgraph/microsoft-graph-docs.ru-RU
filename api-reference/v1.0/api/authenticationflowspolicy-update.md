---
title: Обновление authenticationFlowsPolicy
description: Обновление логического свойства selfServiceSignUp объекта authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d81986c75cb636c45488d2fb35e69b05fdb06e2a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883363"
---
# <a name="update-authenticationflowspolicy"></a><span data-ttu-id="0fff9-103">Обновление authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="0fff9-103">Update authenticationFlowsPolicy</span></span>

<span data-ttu-id="0fff9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fff9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fff9-105">Обновление свойства **selfServiceSignUp** объекта [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fff9-105">Update the **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span> <span data-ttu-id="0fff9-106">Свойства **идентификатор**, **тип** и **описание** изменить невозможно.</span><span class="sxs-lookup"><span data-stu-id="0fff9-106">The properties **id**, **type**, and **description** cannot be modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fff9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fff9-107">Permissions</span></span>

<span data-ttu-id="0fff9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fff9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fff9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fff9-110">Permission type</span></span>|<span data-ttu-id="0fff9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fff9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fff9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fff9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fff9-113">Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="0fff9-113">Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="0fff9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fff9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fff9-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0fff9-115">Not Supported</span></span>|
|<span data-ttu-id="0fff9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fff9-116">Application</span></span>|<span data-ttu-id="0fff9-117">Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="0fff9-117">Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fff9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fff9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="0fff9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fff9-119">Request headers</span></span>

|<span data-ttu-id="0fff9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0fff9-120">Name</span></span>|<span data-ttu-id="0fff9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0fff9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0fff9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fff9-122">Authorization</span></span>|<span data-ttu-id="0fff9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fff9-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0fff9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fff9-125">Content-Type</span></span>|<span data-ttu-id="0fff9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fff9-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fff9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fff9-128">Request body</span></span>

<span data-ttu-id="0fff9-129">В тексте запроса можно указать представление JSON объекта [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fff9-129">In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

<span data-ttu-id="0fff9-130">Ниже показаны свойства, которые необходимо указывать при обновлении[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fff9-130">The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span></span>

|<span data-ttu-id="0fff9-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fff9-131">Property</span></span>|<span data-ttu-id="0fff9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0fff9-132">Type</span></span>|<span data-ttu-id="0fff9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0fff9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fff9-134">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="0fff9-134">selfServiceSignUp</span></span>|[<span data-ttu-id="0fff9-135">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fff9-135">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md)|<span data-ttu-id="0fff9-136">Самостоятельная конфигурация регистрации.</span><span class="sxs-lookup"><span data-stu-id="0fff9-136">Self-service sign-up configuration.</span></span>|

## <a name="response"></a><span data-ttu-id="0fff9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fff9-137">Response</span></span>

<span data-ttu-id="0fff9-138">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="0fff9-138">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fff9-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0fff9-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fff9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fff9-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```

### <a name="response"></a><span data-ttu-id="0fff9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fff9-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

``` http
HTTP/1.1 204 No Content
```
