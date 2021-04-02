---
title: Удаление identityProvider
description: Удаление identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: d78aff8a604f42b7efbc1f87269a87acbb29656c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508829"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="f6bab-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="f6bab-103">Delete identityProvider</span></span>
<span data-ttu-id="f6bab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6bab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6bab-105">Удаление объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f6bab-105">Delete a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="f6bab-106">В Azure AD B2C удалите [объект socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объект appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="f6bab-106">In Azure AD B2C, delete a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6bab-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6bab-107">Permissions</span></span>

<span data-ttu-id="f6bab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6bab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6bab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6bab-110">Permission type</span></span>      | <span data-ttu-id="f6bab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6bab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6bab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6bab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6bab-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bab-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="f6bab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6bab-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f6bab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6bab-115">Not supported.</span></span>|
|<span data-ttu-id="f6bab-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6bab-116">Application</span></span>|<span data-ttu-id="f6bab-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bab-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="f6bab-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f6bab-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f6bab-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f6bab-119">Global Administrator</span></span>
* <span data-ttu-id="f6bab-120">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="f6bab-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f6bab-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6bab-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f6bab-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6bab-122">Request headers</span></span>

|<span data-ttu-id="f6bab-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f6bab-123">Name</span></span>|<span data-ttu-id="f6bab-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f6bab-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f6bab-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6bab-125">Authorization</span></span>|<span data-ttu-id="f6bab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6bab-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6bab-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6bab-128">Request body</span></span>

<span data-ttu-id="f6bab-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6bab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6bab-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6bab-130">Response</span></span>

<span data-ttu-id="f6bab-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f6bab-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6bab-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f6bab-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6bab-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6bab-133">Request</span></span>

<span data-ttu-id="f6bab-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6bab-134">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="f6bab-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6bab-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="f6bab-136">C#</span><span class="sxs-lookup"><span data-stu-id="f6bab-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6bab-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6bab-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6bab-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6bab-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6bab-139">Java</span><span class="sxs-lookup"><span data-stu-id="f6bab-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f6bab-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6bab-140">Response</span></span>

<span data-ttu-id="f6bab-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f6bab-141">The following is an example of the response.</span></span>

<span data-ttu-id="f6bab-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f6bab-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
