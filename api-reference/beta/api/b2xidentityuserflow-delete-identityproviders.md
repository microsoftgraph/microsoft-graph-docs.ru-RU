---
title: Удаление identityProvider из b2xIdentityUserFlow (обесценение)
description: Удаление identityProvider из b2xIdentityUserFlow. (неоконт.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: b596181d0bd74aed6b9d65f932386cc8cb1a9a50
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439723"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow-deprecated"></a><span data-ttu-id="1875e-104">Удаление identityProvider из b2xIdentityUserFlow (обесценение)</span><span class="sxs-lookup"><span data-stu-id="1875e-104">Delete identityProvider from b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="1875e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1875e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="1875e-106">Удаление поставщика удостоверений из [объекта b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="1875e-106">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="1875e-107">Для самообслуживки зарегистрироваться потоки пользователей, значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="1875e-107">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="1875e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1875e-108">Permissions</span></span>

<span data-ttu-id="1875e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1875e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1875e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1875e-111">Permission type</span></span>      | <span data-ttu-id="1875e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1875e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1875e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1875e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1875e-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1875e-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1875e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1875e-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1875e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1875e-116">Not supported.</span></span>|
|<span data-ttu-id="1875e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1875e-117">Application</span></span>| <span data-ttu-id="1875e-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1875e-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1875e-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="1875e-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1875e-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1875e-120">Global administrator</span></span>
* <span data-ttu-id="1875e-121">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="1875e-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1875e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1875e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1875e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1875e-123">Request headers</span></span>

|<span data-ttu-id="1875e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1875e-124">Name</span></span>|<span data-ttu-id="1875e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1875e-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1875e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1875e-126">Authorization</span></span>|<span data-ttu-id="1875e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1875e-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1875e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1875e-129">Request body</span></span>

<span data-ttu-id="1875e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1875e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1875e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1875e-131">Response</span></span>

<span data-ttu-id="1875e-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1875e-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="1875e-133">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="1875e-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="1875e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1875e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="1875e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1875e-135">Request</span></span>

<span data-ttu-id="1875e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1875e-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1875e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1875e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_2"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="1875e-138">C#</span><span class="sxs-lookup"><span data-stu-id="1875e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1875e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1875e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1875e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1875e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1875e-141">Java</span><span class="sxs-lookup"><span data-stu-id="1875e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1875e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1875e-142">Response</span></span>

<span data-ttu-id="1875e-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1875e-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
