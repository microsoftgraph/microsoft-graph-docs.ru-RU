---
title: Список всех identityProviders в b2cIdentityUserFlow
description: Список всех identityProviders в b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: f0d0dbf0cedb1ea267da23301614bd8944da7cdf
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625802"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow"></a><span data-ttu-id="71ce2-103">Список всех identityProviders в b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="71ce2-103">List all identityProviders in a b2cIdentityUserFlow</span></span>

<span data-ttu-id="71ce2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71ce2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71ce2-105">Получите поставщиков удостоверений в [объекте b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="71ce2-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="71ce2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71ce2-106">Permissions</span></span>

<span data-ttu-id="71ce2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ce2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ce2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71ce2-109">Permission type</span></span>      | <span data-ttu-id="71ce2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71ce2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71ce2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71ce2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71ce2-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ce2-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="71ce2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71ce2-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="71ce2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71ce2-114">Not supported.</span></span>|
|<span data-ttu-id="71ce2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="71ce2-115">Application</span></span>| <span data-ttu-id="71ce2-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ce2-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="71ce2-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="71ce2-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="71ce2-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="71ce2-118">Global administrator</span></span>
* <span data-ttu-id="71ce2-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="71ce2-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="71ce2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71ce2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="71ce2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71ce2-121">Request headers</span></span>

|<span data-ttu-id="71ce2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="71ce2-122">Name</span></span>|<span data-ttu-id="71ce2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="71ce2-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="71ce2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71ce2-124">Authorization</span></span>|<span data-ttu-id="71ce2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71ce2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ce2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71ce2-127">Request body</span></span>

<span data-ttu-id="71ce2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71ce2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71ce2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ce2-129">Response</span></span>

<span data-ttu-id="71ce2-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71ce2-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71ce2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="71ce2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="71ce2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="71ce2-132">Request</span></span>

<span data-ttu-id="71ce2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71ce2-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="71ce2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="71ce2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="71ce2-135">C#</span><span class="sxs-lookup"><span data-stu-id="71ce2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71ce2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71ce2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71ce2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71ce2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71ce2-138">Java</span><span class="sxs-lookup"><span data-stu-id="71ce2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71ce2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ce2-139">Response</span></span>

<span data-ttu-id="71ce2-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="71ce2-140">The following is an example of the response.</span></span>

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


