---
title: Удаление emailAuthenticationMethodConfiguration
description: Удаляет объект emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 128148d5402d6ddcd2c95bccf17da7d6cbf379bf
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469299"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="5881d-103">Удаление emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="5881d-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="5881d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5881d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5881d-105">Удалите изменения, внесенные в политику метода проверки [подлинности](../resources/emailauthenticationmethodconfiguration.md) электронной почты, возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5881d-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="5881d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5881d-106">Permissions</span></span>
<span data-ttu-id="5881d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5881d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5881d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5881d-109">Permission type</span></span>|<span data-ttu-id="5881d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5881d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5881d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5881d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5881d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5881d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5881d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5881d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5881d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5881d-114">Not supported.</span></span>|
|<span data-ttu-id="5881d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5881d-115">Application</span></span>|<span data-ttu-id="5881d-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5881d-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="5881d-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="5881d-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="5881d-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="5881d-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="5881d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5881d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="5881d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5881d-120">Request headers</span></span>

|<span data-ttu-id="5881d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5881d-121">Name</span></span>|<span data-ttu-id="5881d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5881d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5881d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5881d-123">Authorization</span></span>|<span data-ttu-id="5881d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5881d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5881d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5881d-126">Request body</span></span>

<span data-ttu-id="5881d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5881d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5881d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5881d-128">Response</span></span>

<span data-ttu-id="5881d-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5881d-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5881d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5881d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5881d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5881d-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5881d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5881d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```
# <a name="c"></a>[<span data-ttu-id="5881d-133">C#</span><span class="sxs-lookup"><span data-stu-id="5881d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5881d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5881d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5881d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5881d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5881d-136">Java</span><span class="sxs-lookup"><span data-stu-id="5881d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5881d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5881d-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

