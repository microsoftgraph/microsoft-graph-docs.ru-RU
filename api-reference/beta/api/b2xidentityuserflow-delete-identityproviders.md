---
title: Удаление identityProvider из b2xIdentityUserFlow
description: Удаление объекта identityProvider из b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 751a4a5c351126a47f3a6962e951e0cf6a24b178
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406376"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow"></a><span data-ttu-id="f287f-103">Удаление identityProvider из b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="f287f-103">Delete identityProvider from b2xIdentityUserFlow</span></span>

<span data-ttu-id="f287f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f287f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f287f-105">Удаление поставщика удостоверений из объекта [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="f287f-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="f287f-106">Для самостоятельной регистрации пользовательских потоков значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="f287f-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f287f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f287f-107">Permissions</span></span>

<span data-ttu-id="f287f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f287f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f287f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f287f-110">Permission type</span></span>      | <span data-ttu-id="f287f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f287f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f287f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f287f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f287f-113">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f287f-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f287f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f287f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f287f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f287f-115">Not supported.</span></span>|
|<span data-ttu-id="f287f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f287f-116">Application</span></span>| <span data-ttu-id="f287f-117">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f287f-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f287f-118">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f287f-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f287f-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f287f-119">Global administrator</span></span>
* <span data-ttu-id="f287f-120">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="f287f-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f287f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f287f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f287f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f287f-122">Request headers</span></span>

|<span data-ttu-id="f287f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f287f-123">Name</span></span>|<span data-ttu-id="f287f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f287f-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f287f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f287f-125">Authorization</span></span>|<span data-ttu-id="f287f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f287f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f287f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f287f-128">Request body</span></span>

<span data-ttu-id="f287f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f287f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f287f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f287f-130">Response</span></span>

<span data-ttu-id="f287f-131">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f287f-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="f287f-132">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="f287f-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f287f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f287f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f287f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f287f-134">Request</span></span>

<span data-ttu-id="f287f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f287f-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f287f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f287f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="f287f-137">C#</span><span class="sxs-lookup"><span data-stu-id="f287f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f287f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f287f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f287f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f287f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f287f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f287f-140">Response</span></span>

<span data-ttu-id="f287f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f287f-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


