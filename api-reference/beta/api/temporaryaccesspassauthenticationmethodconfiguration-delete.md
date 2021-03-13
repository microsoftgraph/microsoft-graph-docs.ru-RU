---
title: Удаление temporaryAccessPassAuthenticationMethodConfiguration
description: Удалите изменения, внесенные в объект temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f55afafed3863ffeab1c8bf786602606112e048b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761858"
---
# <a name="delete-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="3d59d-103">Удаление temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d59d-103">Delete temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="3d59d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d59d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d59d-105">Удалите изменения, внесенные в [объект temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) возвращая политику к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3d59d-105">Remove changes made to the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d59d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d59d-106">Permissions</span></span>
<span data-ttu-id="3d59d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d59d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d59d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d59d-109">Permission type</span></span>|<span data-ttu-id="3d59d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d59d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d59d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d59d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d59d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3d59d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="3d59d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d59d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d59d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d59d-114">Not supported.</span></span>|
|<span data-ttu-id="3d59d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d59d-115">Application</span></span>|<span data-ttu-id="3d59d-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3d59d-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="3d59d-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="3d59d-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="3d59d-118">Дополнительные сведения см. в [дополнительных сведениях.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="3d59d-118">For more information, see [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="3d59d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d59d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


## <a name="request-headers"></a><span data-ttu-id="3d59d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d59d-120">Request headers</span></span>
|<span data-ttu-id="3d59d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3d59d-121">Name</span></span>|<span data-ttu-id="3d59d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3d59d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3d59d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d59d-123">Authorization</span></span>|<span data-ttu-id="3d59d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d59d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d59d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d59d-126">Request body</span></span>
<span data-ttu-id="3d59d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d59d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d59d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d59d-128">Response</span></span>

<span data-ttu-id="3d59d-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3d59d-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3d59d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d59d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d59d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d59d-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3d59d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d59d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
# <a name="c"></a>[<span data-ttu-id="3d59d-133">C#</span><span class="sxs-lookup"><span data-stu-id="3d59d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d59d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d59d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d59d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d59d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d59d-136">Java</span><span class="sxs-lookup"><span data-stu-id="3d59d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3d59d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d59d-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
