---
title: Удаление MicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Удаляет объект MicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93a16ae2865fcdb85963c7e8aded8e5ca6727720
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202759"
---
# <a name="delete-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="024dd-103">Удаление MicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="024dd-103">Delete microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="024dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="024dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="024dd-105">Удалите изменения, внесенные в политику проверки подлинности [Microsoft Authenticator,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="024dd-105">Remove changes made to the [Microsoft Authenticator authentication method policy](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="024dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="024dd-106">Permissions</span></span>
<span data-ttu-id="024dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="024dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="024dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="024dd-109">Permission type</span></span>|<span data-ttu-id="024dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="024dd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="024dd-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="024dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="024dd-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="024dd-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="024dd-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="024dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="024dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="024dd-114">Not supported.</span></span>|
|<span data-ttu-id="024dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="024dd-115">Application</span></span>|<span data-ttu-id="024dd-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="024dd-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="024dd-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="024dd-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="024dd-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="024dd-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="024dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="024dd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="024dd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="024dd-120">Request headers</span></span>
|<span data-ttu-id="024dd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="024dd-121">Name</span></span>|<span data-ttu-id="024dd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="024dd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="024dd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="024dd-123">Authorization</span></span>|<span data-ttu-id="024dd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="024dd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="024dd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="024dd-126">Request body</span></span>
<span data-ttu-id="024dd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="024dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="024dd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="024dd-128">Response</span></span>

<span data-ttu-id="024dd-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="024dd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="024dd-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="024dd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="024dd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="024dd-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="024dd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="024dd-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```
# <a name="c"></a>[<span data-ttu-id="024dd-133">C#</span><span class="sxs-lookup"><span data-stu-id="024dd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-microsoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="024dd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="024dd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-microsoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="024dd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="024dd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-microsoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="024dd-136">Java</span><span class="sxs-lookup"><span data-stu-id="024dd-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-microsoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="024dd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="024dd-137">Response</span></span>
<span data-ttu-id="024dd-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="024dd-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

