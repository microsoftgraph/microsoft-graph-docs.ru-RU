---
title: Удаление identityProvider из b2cIdentityUserFlow (обесценение)
description: Удаление identityProvider из b2cIdentityUserFlow. (неоконт.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 64a72b0d286ff9e794d8ca654d498ee95f1a52de
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439814"
---
# <a name="delete-an-identityprovider-from-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="0698b-104">Удаление идентификатораProvider из b2cIdentityUserFlow (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="0698b-104">Delete an identityProvider from a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="0698b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0698b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="0698b-106">Удаление поставщика удостоверений из [объекта b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="0698b-106">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="0698b-107">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в справке об API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="0698b-107">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="0698b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0698b-108">Permissions</span></span>

<span data-ttu-id="0698b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0698b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0698b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0698b-111">Permission type</span></span>      | <span data-ttu-id="0698b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0698b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0698b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0698b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0698b-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0698b-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0698b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0698b-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0698b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0698b-116">Not supported.</span></span>|
|<span data-ttu-id="0698b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0698b-117">Application</span></span>| <span data-ttu-id="0698b-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0698b-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0698b-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="0698b-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0698b-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0698b-120">Global administrator</span></span>
* <span data-ttu-id="0698b-121">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="0698b-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0698b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0698b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0698b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0698b-123">Request headers</span></span>

|<span data-ttu-id="0698b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0698b-124">Name</span></span>|<span data-ttu-id="0698b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0698b-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0698b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0698b-126">Authorization</span></span>|<span data-ttu-id="0698b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0698b-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0698b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0698b-129">Request body</span></span>

<span data-ttu-id="0698b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0698b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0698b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0698b-131">Response</span></span>

<span data-ttu-id="0698b-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0698b-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="0698b-133">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="0698b-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="0698b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0698b-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="0698b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0698b-135">Request</span></span>

<span data-ttu-id="0698b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0698b-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0698b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0698b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_1"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="0698b-138">C#</span><span class="sxs-lookup"><span data-stu-id="0698b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0698b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0698b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0698b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0698b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0698b-141">Java</span><span class="sxs-lookup"><span data-stu-id="0698b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0698b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0698b-142">Response</span></span>

<span data-ttu-id="0698b-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0698b-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
