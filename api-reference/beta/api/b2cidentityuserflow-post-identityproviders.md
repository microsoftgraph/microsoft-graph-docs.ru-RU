---
title: Добавление identityProvider в b2cIdentityUserFlow
description: Добавьте identityProvider в b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4c6dcfc7dc1dce6866585b789539c17099eb8214
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047968"
---
# <a name="add-identityprovider-to-a-b2cidentityuserflow"></a><span data-ttu-id="f56b8-103">Добавление identityProvider в b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="f56b8-103">Add identityProvider to a b2cIdentityUserFlow</span></span>

<span data-ttu-id="f56b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f56b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f56b8-105">Добавление поставщиков удостоверений в [объект b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f56b8-105">Add identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f56b8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f56b8-106">Permissions</span></span>

<span data-ttu-id="f56b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f56b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f56b8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f56b8-109">Permission type</span></span>      | <span data-ttu-id="f56b8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f56b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f56b8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f56b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f56b8-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f56b8-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f56b8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f56b8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f56b8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f56b8-114">Not supported.</span></span>|
|<span data-ttu-id="f56b8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f56b8-115">Application</span></span>| <span data-ttu-id="f56b8-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f56b8-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f56b8-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f56b8-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f56b8-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f56b8-118">Global administrator</span></span>
* <span data-ttu-id="f56b8-119">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="f56b8-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f56b8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f56b8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f56b8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f56b8-121">Request headers</span></span>

|<span data-ttu-id="f56b8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f56b8-122">Name</span></span>|<span data-ttu-id="f56b8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f56b8-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f56b8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f56b8-124">Authorization</span></span>|<span data-ttu-id="f56b8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f56b8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f56b8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f56b8-127">Content-Type</span></span>|<span data-ttu-id="f56b8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f56b8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f56b8-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f56b8-130">Request body</span></span>

<span data-ttu-id="f56b8-131">В теле запроса предопрейте JSON представление `id` [идентификатораProvider,](../resources/identityprovider.md) который необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="f56b8-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="f56b8-132">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в справке об API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="f56b8-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="f56b8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f56b8-133">Response</span></span>

<span data-ttu-id="f56b8-134">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f56b8-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="f56b8-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="f56b8-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f56b8-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f56b8-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="f56b8-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f56b8-137">Request</span></span>

<span data-ttu-id="f56b8-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f56b8-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f56b8-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f56b8-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="f56b8-140">C#</span><span class="sxs-lookup"><span data-stu-id="f56b8-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f56b8-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f56b8-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f56b8-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f56b8-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f56b8-143">Java</span><span class="sxs-lookup"><span data-stu-id="f56b8-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f56b8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f56b8-144">Response</span></span>

<span data-ttu-id="f56b8-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f56b8-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
