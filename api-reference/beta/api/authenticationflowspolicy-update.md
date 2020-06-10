---
title: Обновление Аусентикатионфловсполици
description: Обновление логического свойства Селфсервицесигнуп объекта Аусентикатионфловсполици.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3408cff98cc79dbf819e077ab12fa066f7d723f7
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680896"
---
# <a name="update-authenticationflowspolicy"></a><span data-ttu-id="62691-103">Обновление Аусентикатионфловсполици</span><span class="sxs-lookup"><span data-stu-id="62691-103">Update authenticationFlowsPolicy</span></span>

<span data-ttu-id="62691-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62691-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62691-105">Обновление логического свойства **селфсервицесигнуп** объекта [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="62691-105">Update the Boolean **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span> <span data-ttu-id="62691-106">**Идентификатор**, **тип**и **Описание** свойства не могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62691-106">The properties **id**, **type**, and **description** cannot be modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="62691-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62691-107">Permissions</span></span>
<span data-ttu-id="62691-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62691-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62691-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62691-110">Permission type</span></span>|<span data-ttu-id="62691-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62691-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62691-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62691-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62691-113">Policy. ReadWrite. Аусентикатионфловс</span><span class="sxs-lookup"><span data-stu-id="62691-113">Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="62691-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62691-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62691-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="62691-115">Not Supported</span></span>|
|<span data-ttu-id="62691-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62691-116">Application</span></span>|<span data-ttu-id="62691-117">Policy. ReadWrite. Аусентикатионфловс</span><span class="sxs-lookup"><span data-stu-id="62691-117">Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="62691-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62691-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="62691-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62691-119">Request headers</span></span>
|<span data-ttu-id="62691-120">Имя</span><span class="sxs-lookup"><span data-stu-id="62691-120">Name</span></span>|<span data-ttu-id="62691-121">Описание</span><span class="sxs-lookup"><span data-stu-id="62691-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="62691-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62691-122">Authorization</span></span>|<span data-ttu-id="62691-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62691-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="62691-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62691-125">Content-Type</span></span>|<span data-ttu-id="62691-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62691-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62691-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="62691-128">Request body</span></span>
<span data-ttu-id="62691-129">В тексте запроса вы можете предоставить представление объекта [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) в формате JSON (необязательно).</span><span class="sxs-lookup"><span data-stu-id="62691-129">In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object (but is not required.)</span></span>

<span data-ttu-id="62691-130">В следующей таблице приведены свойства, необходимые при обновлении [аусентикатионфловсполици](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62691-130">The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span></span>

|<span data-ttu-id="62691-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="62691-131">Property</span></span>|<span data-ttu-id="62691-132">Тип</span><span class="sxs-lookup"><span data-stu-id="62691-132">Type</span></span>|<span data-ttu-id="62691-133">Описание</span><span class="sxs-lookup"><span data-stu-id="62691-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62691-134">селфсервицесигнуп</span><span class="sxs-lookup"><span data-stu-id="62691-134">selfServiceSignUp</span></span>|[<span data-ttu-id="62691-135">селфсервицесигнупаусентикатионфловконфигуратион</span><span class="sxs-lookup"><span data-stu-id="62691-135">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md)|<span data-ttu-id="62691-136">Самостоятельная настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="62691-136">Self-service sign-up configuration.</span></span>|

## <a name="response"></a><span data-ttu-id="62691-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="62691-137">Response</span></span>

<span data-ttu-id="62691-138">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="62691-138">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="62691-139">Пример</span><span class="sxs-lookup"><span data-stu-id="62691-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="62691-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="62691-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="62691-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="62691-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->
```http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="62691-142">C#</span><span class="sxs-lookup"><span data-stu-id="62691-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62691-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62691-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62691-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62691-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62691-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="62691-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```
