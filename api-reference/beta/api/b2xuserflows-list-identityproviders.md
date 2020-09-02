---
title: Перечисление всех Идентитипровидерс в b2xUserFlow
description: Перечисление всех Идентитипровидерс в b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad71b925d8fc2d36e997a1367497414f2feead7a
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329414"
---
# <a name="list-all-identityproviders-in-a-b2xuserflow"></a><span data-ttu-id="bb3c4-103">Перечисление всех Идентитипровидерс в b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="bb3c4-103">List all identityProviders in a b2xUserFlow</span></span>

<span data-ttu-id="bb3c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb3c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb3c4-105">Получение поставщиков удостоверений в объекте [b2xUserFlow](../resources/b2xuserflows.md)</span><span class="sxs-lookup"><span data-stu-id="bb3c4-105">Get the identity providers in a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb3c4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb3c4-106">Permissions</span></span>

<span data-ttu-id="bb3c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb3c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb3c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb3c4-109">Permission type</span></span>      | <span data-ttu-id="bb3c4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb3c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb3c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb3c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb3c4-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bb3c4-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="bb3c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb3c4-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bb3c4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb3c4-114">Not supported.</span></span>|
|<span data-ttu-id="bb3c4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb3c4-115">Application</span></span>| <span data-ttu-id="bb3c4-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bb3c4-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="bb3c4-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="bb3c4-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bb3c4-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="bb3c4-118">Global administrator</span></span>
* <span data-ttu-id="bb3c4-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="bb3c4-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bb3c4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb3c4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="bb3c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb3c4-121">Request headers</span></span>

|<span data-ttu-id="bb3c4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bb3c4-122">Name</span></span>|<span data-ttu-id="bb3c4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bb3c4-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bb3c4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb3c4-124">Authorization</span></span>|<span data-ttu-id="bb3c4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb3c4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb3c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb3c4-127">Request body</span></span>

<span data-ttu-id="bb3c4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb3c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb3c4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb3c4-129">Response</span></span>

<span data-ttu-id="bb3c4-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [идентитипровидерс](../resources/identityprovider.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb3c4-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb3c4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb3c4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb3c4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb3c4-132">Request</span></span>

<span data-ttu-id="bb3c4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb3c4-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bb3c4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb3c4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="bb3c4-135">C#</span><span class="sxs-lookup"><span data-stu-id="bb3c4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb3c4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb3c4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb3c4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb3c4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb3c4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb3c4-138">Response</span></span>

<span data-ttu-id="bb3c4-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bb3c4-139">The following is an example of the response.</span></span>

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
