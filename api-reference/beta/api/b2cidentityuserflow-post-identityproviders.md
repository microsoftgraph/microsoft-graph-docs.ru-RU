---
title: Добавление identityProvider в b2cIdentityUserFlow (обесценение)
description: Добавьте identityProvider в b2cIdentityUserFlow. (неоконт.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9a5591465329d879a4a1bd3e4b0028cad2b6cdef
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439737"
---
# <a name="add-identityprovider-to-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="3de88-104">Добавление identityProvider в b2cIdentityUserFlow (обесценение)</span><span class="sxs-lookup"><span data-stu-id="3de88-104">Add identityProvider to a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="3de88-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3de88-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="3de88-106">Добавление поставщиков удостоверений в [объект b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="3de88-106">Add identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3de88-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3de88-107">Permissions</span></span>

<span data-ttu-id="3de88-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3de88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de88-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3de88-110">Permission type</span></span>      | <span data-ttu-id="3de88-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3de88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3de88-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3de88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3de88-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de88-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3de88-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3de88-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3de88-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de88-115">Not supported.</span></span>|
|<span data-ttu-id="3de88-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3de88-116">Application</span></span>| <span data-ttu-id="3de88-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de88-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3de88-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="3de88-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3de88-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3de88-119">Global administrator</span></span>
* <span data-ttu-id="3de88-120">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="3de88-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3de88-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3de88-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3de88-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3de88-122">Request headers</span></span>

|<span data-ttu-id="3de88-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3de88-123">Name</span></span>|<span data-ttu-id="3de88-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3de88-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3de88-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3de88-125">Authorization</span></span>|<span data-ttu-id="3de88-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3de88-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3de88-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3de88-128">Content-Type</span></span>|<span data-ttu-id="3de88-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3de88-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3de88-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3de88-131">Request body</span></span>

<span data-ttu-id="3de88-132">В теле запроса предопрейте JSON представление `id` [идентификатораProvider,](../resources/identityprovider.md) который необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="3de88-132">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="3de88-133">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в справке об API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="3de88-133">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="3de88-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de88-134">Response</span></span>

<span data-ttu-id="3de88-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3de88-135">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="3de88-136">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="3de88-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="3de88-137">Пример</span><span class="sxs-lookup"><span data-stu-id="3de88-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3de88-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="3de88-138">Request</span></span>

<span data-ttu-id="3de88-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3de88-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3de88-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3de88-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3de88-141">C#</span><span class="sxs-lookup"><span data-stu-id="3de88-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3de88-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3de88-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3de88-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3de88-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3de88-144">Java</span><span class="sxs-lookup"><span data-stu-id="3de88-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3de88-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de88-145">Response</span></span>

<span data-ttu-id="3de88-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3de88-146">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
