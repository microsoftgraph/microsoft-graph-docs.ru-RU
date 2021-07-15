---
title: Удаление userFlowIdentityProvider
description: Удаление identityProvider из b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 85fff2d0fab5d9d098aa7cae780c99faece3916f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439679"
---
# <a name="delete-a-userflowidentityprovider"></a><span data-ttu-id="e966f-103">Удаление userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="e966f-103">Delete a userFlowIdentityProvider</span></span>

<span data-ttu-id="e966f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e966f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e966f-105">Удаление поставщика удостоверений из [объекта b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="e966f-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="e966f-106">Для самообслуживки зарегистрироваться потоки пользователей, значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="e966f-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e966f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e966f-107">Permissions</span></span>

<span data-ttu-id="e966f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e966f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e966f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e966f-110">Permission type</span></span>      | <span data-ttu-id="e966f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e966f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e966f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e966f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e966f-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e966f-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e966f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e966f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e966f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e966f-115">Not supported.</span></span>|
|<span data-ttu-id="e966f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e966f-116">Application</span></span>| <span data-ttu-id="e966f-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e966f-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e966f-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="e966f-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e966f-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e966f-119">Global administrator</span></span>
* <span data-ttu-id="e966f-120">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="e966f-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e966f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e966f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e966f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e966f-122">Request headers</span></span>

|<span data-ttu-id="e966f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e966f-123">Name</span></span>|<span data-ttu-id="e966f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e966f-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e966f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e966f-125">Authorization</span></span>|<span data-ttu-id="e966f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e966f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e966f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e966f-128">Request body</span></span>

<span data-ttu-id="e966f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e966f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e966f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e966f-130">Response</span></span>

<span data-ttu-id="e966f-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e966f-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="e966f-132">В случае `4xx` неудачи возвращается ошибка с определенными сведениями об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e966f-132">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="e966f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e966f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e966f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e966f-134">Request</span></span>

<span data-ttu-id="e966f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e966f-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e966f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e966f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="e966f-137">C#</span><span class="sxs-lookup"><span data-stu-id="e966f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e966f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e966f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e966f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e966f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e966f-140">Java</span><span class="sxs-lookup"><span data-stu-id="e966f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e966f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e966f-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
