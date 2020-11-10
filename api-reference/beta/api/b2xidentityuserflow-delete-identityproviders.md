---
title: Удаление identityProvider из b2xIdentityUserFlow
description: Удаление объекта identityProvider из b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 25db32f3f84a705f167fe1216b2a68554d9e3e9e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961141"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow"></a><span data-ttu-id="40ef0-103">Удаление identityProvider из b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="40ef0-103">Delete identityProvider from b2xIdentityUserFlow</span></span>

<span data-ttu-id="40ef0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ef0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40ef0-105">Удаление поставщика удостоверений из объекта [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="40ef0-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="40ef0-106">Для самостоятельной регистрации пользовательских потоков значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="40ef0-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="40ef0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40ef0-107">Permissions</span></span>

<span data-ttu-id="40ef0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ef0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ef0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40ef0-110">Permission type</span></span>      | <span data-ttu-id="40ef0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40ef0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40ef0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40ef0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40ef0-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ef0-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="40ef0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40ef0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="40ef0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ef0-115">Not supported.</span></span>|
|<span data-ttu-id="40ef0-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="40ef0-116">Application</span></span>| <span data-ttu-id="40ef0-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ef0-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="40ef0-118">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="40ef0-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="40ef0-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="40ef0-119">Global administrator</span></span>
* <span data-ttu-id="40ef0-120">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="40ef0-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="40ef0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40ef0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="40ef0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40ef0-122">Request headers</span></span>

|<span data-ttu-id="40ef0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="40ef0-123">Name</span></span>|<span data-ttu-id="40ef0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="40ef0-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="40ef0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40ef0-125">Authorization</span></span>|<span data-ttu-id="40ef0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40ef0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ef0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40ef0-128">Request body</span></span>

<span data-ttu-id="40ef0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40ef0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40ef0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ef0-130">Response</span></span>

<span data-ttu-id="40ef0-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="40ef0-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="40ef0-132">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="40ef0-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="40ef0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="40ef0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="40ef0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="40ef0-134">Request</span></span>

<span data-ttu-id="40ef0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40ef0-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="40ef0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="40ef0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="40ef0-137">C#</span><span class="sxs-lookup"><span data-stu-id="40ef0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40ef0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40ef0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40ef0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40ef0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40ef0-140">Java</span><span class="sxs-lookup"><span data-stu-id="40ef0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40ef0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ef0-141">Response</span></span>

<span data-ttu-id="40ef0-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="40ef0-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


