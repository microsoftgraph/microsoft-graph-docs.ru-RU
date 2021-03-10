---
title: Добавление identityProvider в b2xIdentityUserFlow
description: Добавьте identityProvider в b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: db326c4fe3ed63b4387d7fb5414312d683f26322
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625724"
---
# <a name="add-identityprovider-to-a-b2xidentityuserflow"></a><span data-ttu-id="689d1-103">Добавление identityProvider в b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="689d1-103">Add identityProvider to a b2xIdentityUserFlow</span></span>

<span data-ttu-id="689d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="689d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="689d1-105">Обновление поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="689d1-105">Update the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="689d1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="689d1-106">Permissions</span></span>

<span data-ttu-id="689d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="689d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="689d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="689d1-109">Permission type</span></span>      | <span data-ttu-id="689d1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="689d1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="689d1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="689d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="689d1-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689d1-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="689d1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="689d1-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="689d1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="689d1-114">Not supported.</span></span>|
|<span data-ttu-id="689d1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="689d1-115">Application</span></span>| <span data-ttu-id="689d1-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689d1-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="689d1-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="689d1-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="689d1-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="689d1-118">Global administrator</span></span>
* <span data-ttu-id="689d1-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="689d1-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="689d1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="689d1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="689d1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="689d1-121">Request headers</span></span>

|<span data-ttu-id="689d1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="689d1-122">Name</span></span>|<span data-ttu-id="689d1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="689d1-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="689d1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="689d1-124">Authorization</span></span>|<span data-ttu-id="689d1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="689d1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="689d1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="689d1-127">Content-Type</span></span>|<span data-ttu-id="689d1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="689d1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="689d1-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="689d1-130">Request body</span></span>

<span data-ttu-id="689d1-131">В теле запроса предопрейте JSON представление `id` [идентификатораProvider,](../resources/identityprovider.md) который необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="689d1-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="689d1-132">Для самообслуживки зарегистрироваться потоки пользователей, значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="689d1-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="689d1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="689d1-133">Response</span></span>

<span data-ttu-id="689d1-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="689d1-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="689d1-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="689d1-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="689d1-136">Пример</span><span class="sxs-lookup"><span data-stu-id="689d1-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="689d1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="689d1-137">Request</span></span>

<span data-ttu-id="689d1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="689d1-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="689d1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="689d1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="689d1-140">C#</span><span class="sxs-lookup"><span data-stu-id="689d1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2xuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="689d1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="689d1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2xuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="689d1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="689d1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2xuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="689d1-143">Java</span><span class="sxs-lookup"><span data-stu-id="689d1-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2xuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="689d1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="689d1-144">Response</span></span>

<span data-ttu-id="689d1-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="689d1-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


