---
title: Удаление temporaryAccessPassAuthenticationMethodConfiguration
description: Удалите изменения, внесенные в объект temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4512b4127a9c1fe1bab4c9e7bc0645d39f79c3b1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954003"
---
# <a name="delete-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="cdc3a-103">Удаление temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="cdc3a-103">Delete temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="cdc3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc3a-105">Удалите изменения, внесенные в [объект temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) возвращая политику к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cdc3a-105">Remove changes made to the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc3a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdc3a-106">Permissions</span></span>
<span data-ttu-id="cdc3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc3a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdc3a-109">Permission type</span></span>|<span data-ttu-id="cdc3a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdc3a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdc3a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdc3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdc3a-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cdc3a-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="cdc3a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdc3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdc3a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdc3a-114">Not supported.</span></span>|
|<span data-ttu-id="cdc3a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdc3a-115">Application</span></span>|<span data-ttu-id="cdc3a-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cdc3a-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="cdc3a-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="cdc3a-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="cdc3a-118">Дополнительные сведения см. в [дополнительных сведениях.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="cdc3a-118">For more information, see [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="cdc3a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdc3a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


## <a name="request-headers"></a><span data-ttu-id="cdc3a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdc3a-120">Request headers</span></span>
|<span data-ttu-id="cdc3a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cdc3a-121">Name</span></span>|<span data-ttu-id="cdc3a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cdc3a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cdc3a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdc3a-123">Authorization</span></span>|<span data-ttu-id="cdc3a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdc3a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdc3a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdc3a-126">Request body</span></span>
<span data-ttu-id="cdc3a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdc3a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc3a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdc3a-128">Response</span></span>

<span data-ttu-id="cdc3a-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cdc3a-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cdc3a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cdc3a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdc3a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdc3a-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cdc3a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc3a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration_2"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
# <a name="c"></a>[<span data-ttu-id="cdc3a-133">C#</span><span class="sxs-lookup"><span data-stu-id="cdc3a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethodconfiguration-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc3a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc3a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethodconfiguration-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc3a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc3a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethodconfiguration-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc3a-136">Java</span><span class="sxs-lookup"><span data-stu-id="cdc3a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethodconfiguration-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cdc3a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdc3a-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
