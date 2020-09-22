---
title: Удаление identityProvider из b2cUserFlow
description: Удаление объекта identityProvider из b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae6b285ee748b3391a80120c17d4535c534b4893
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991532"
---
# <a name="delete-an-identityprovider-from-a-b2cuserflow"></a><span data-ttu-id="e3ceb-103">Удаление объекта identityProvider из b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="e3ceb-103">Delete an identityProvider from a b2cUserFlow</span></span>

<span data-ttu-id="e3ceb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3ceb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3ceb-105">Удаление поставщика удостоверений из объекта [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="e3ceb-105">Delete an identity provider from a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span> <span data-ttu-id="e3ceb-106">Дополнительные сведения о поставщиках удостоверений, доступных для пользовательских потоков, представлены в справочнике по API [идентитипровидерс](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="e3ceb-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3ceb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3ceb-107">Permissions</span></span>

<span data-ttu-id="e3ceb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3ceb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3ceb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3ceb-110">Permission type</span></span>      | <span data-ttu-id="e3ceb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3ceb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3ceb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3ceb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3ceb-113">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e3ceb-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e3ceb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3ceb-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e3ceb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3ceb-115">Not supported.</span></span>|
|<span data-ttu-id="e3ceb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3ceb-116">Application</span></span>| <span data-ttu-id="e3ceb-117">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e3ceb-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e3ceb-118">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="e3ceb-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e3ceb-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e3ceb-119">Global administrator</span></span>
* <span data-ttu-id="e3ceb-120">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="e3ceb-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e3ceb-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3ceb-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e3ceb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3ceb-122">Request headers</span></span>

|<span data-ttu-id="e3ceb-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e3ceb-123">Name</span></span>|<span data-ttu-id="e3ceb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e3ceb-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e3ceb-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3ceb-125">Authorization</span></span>|<span data-ttu-id="e3ceb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3ceb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3ceb-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3ceb-128">Request body</span></span>

<span data-ttu-id="e3ceb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3ceb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3ceb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3ceb-130">Response</span></span>

<span data-ttu-id="e3ceb-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e3ceb-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="e3ceb-132">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="e3ceb-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="e3ceb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e3ceb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3ceb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3ceb-134">Request</span></span>

<span data-ttu-id="e3ceb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3ceb-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e3ceb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3ceb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="e3ceb-137">C#</span><span class="sxs-lookup"><span data-stu-id="e3ceb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3ceb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3ceb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3ceb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3ceb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e3ceb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3ceb-140">Response</span></span>

<span data-ttu-id="e3ceb-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e3ceb-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


