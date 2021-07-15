---
title: Добавление userFlowIdentityProvider
description: Добавьте identityProvider в b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: c183cd97377004d60485dcacf0bf372f8957f0b8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439710"
---
# <a name="add-a-userflowidentityprovider"></a><span data-ttu-id="7cf46-103">Добавление userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="7cf46-103">Add a userFlowIdentityProvider</span></span>

<span data-ttu-id="7cf46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cf46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cf46-105">Добавьте поставщиков удостоверений в [объект b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="7cf46-105">Add an identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cf46-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cf46-106">Permissions</span></span>

<span data-ttu-id="7cf46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cf46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cf46-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cf46-109">Permission type</span></span>      | <span data-ttu-id="7cf46-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cf46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cf46-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cf46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7cf46-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf46-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7cf46-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cf46-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7cf46-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cf46-114">Not supported.</span></span>|
|<span data-ttu-id="7cf46-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7cf46-115">Application</span></span>| <span data-ttu-id="7cf46-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf46-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7cf46-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="7cf46-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7cf46-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7cf46-118">Global administrator</span></span>
* <span data-ttu-id="7cf46-119">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="7cf46-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7cf46-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cf46-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7cf46-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cf46-121">Request headers</span></span>

|<span data-ttu-id="7cf46-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7cf46-122">Name</span></span>|<span data-ttu-id="7cf46-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf46-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7cf46-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7cf46-124">Authorization</span></span>|<span data-ttu-id="7cf46-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cf46-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7cf46-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7cf46-127">Content-Type</span></span>|<span data-ttu-id="7cf46-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cf46-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cf46-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cf46-130">Request body</span></span>

<span data-ttu-id="7cf46-131">В теле запроса предопрейте представление JSON с идентификатором, который `id` необходимо добавить. [](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="7cf46-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="7cf46-132">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в [ресурсе identityProviders.](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="7cf46-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="7cf46-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cf46-133">Response</span></span>

<span data-ttu-id="7cf46-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7cf46-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="7cf46-135">В случае `4xx` неудачи возвращается ошибка с определенными сведениями об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7cf46-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="7cf46-136">Пример</span><span class="sxs-lookup"><span data-stu-id="7cf46-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cf46-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cf46-137">Request</span></span>

<span data-ttu-id="7cf46-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cf46-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7cf46-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf46-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_userflowIdentityProviders"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="7cf46-140">C#</span><span class="sxs-lookup"><span data-stu-id="7cf46-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cf46-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cf46-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cf46-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cf46-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cf46-143">Java</span><span class="sxs-lookup"><span data-stu-id="7cf46-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7cf46-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cf46-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
