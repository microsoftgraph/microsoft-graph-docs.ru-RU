---
title: Список всех identityProviders в b2cIdentityUserFlow (обесценив)
description: Список всех identityProviders в b2cIdentityUserFlow. (неоконт.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 56ed128f253df192b2fdabb38930883c4b2c8c6b
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439779"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="a434f-104">Список всех identityProviders в b2cIdentityUserFlow (обесценив)</span><span class="sxs-lookup"><span data-stu-id="a434f-104">List all identityProviders in a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="a434f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a434f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="a434f-106">Получите поставщиков удостоверений в [объекте b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="a434f-106">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a434f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a434f-107">Permissions</span></span>

<span data-ttu-id="a434f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a434f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a434f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a434f-110">Permission type</span></span>      | <span data-ttu-id="a434f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a434f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a434f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a434f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a434f-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a434f-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a434f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a434f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a434f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a434f-115">Not supported.</span></span>|
|<span data-ttu-id="a434f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a434f-116">Application</span></span>| <span data-ttu-id="a434f-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a434f-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a434f-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="a434f-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a434f-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a434f-119">Global administrator</span></span>
* <span data-ttu-id="a434f-120">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="a434f-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a434f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a434f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="a434f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a434f-122">Request headers</span></span>

|<span data-ttu-id="a434f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a434f-123">Name</span></span>|<span data-ttu-id="a434f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a434f-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a434f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a434f-125">Authorization</span></span>|<span data-ttu-id="a434f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a434f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a434f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a434f-128">Request body</span></span>

<span data-ttu-id="a434f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a434f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a434f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a434f-130">Response</span></span>

<span data-ttu-id="a434f-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a434f-131">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a434f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a434f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a434f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a434f-133">Request</span></span>

<span data-ttu-id="a434f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a434f-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a434f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a434f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="a434f-136">C#</span><span class="sxs-lookup"><span data-stu-id="a434f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a434f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a434f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a434f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a434f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a434f-139">Java</span><span class="sxs-lookup"><span data-stu-id="a434f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a434f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a434f-140">Response</span></span>

<span data-ttu-id="a434f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a434f-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "*****"
        },
        {
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}
```
