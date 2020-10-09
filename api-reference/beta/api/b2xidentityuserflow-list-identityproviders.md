---
title: Перечисление всех Идентитипровидерс в b2xIdentityUserFlow
description: Перечисление всех Идентитипровидерс в b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b0bb3f93df0b1de9c6ccd209a67d65781d9c7fda
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406440"
---
# <a name="list-all-identityproviders-in-a-b2xidentityuserflow"></a><span data-ttu-id="8da4d-103">Перечисление всех Идентитипровидерс в b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="8da4d-103">List all identityProviders in a b2xIdentityUserFlow</span></span>

<span data-ttu-id="8da4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8da4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8da4d-105">Получение поставщиков удостоверений в объекте [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="8da4d-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8da4d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8da4d-106">Permissions</span></span>

<span data-ttu-id="8da4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8da4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8da4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8da4d-109">Permission type</span></span>      | <span data-ttu-id="8da4d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8da4d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8da4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8da4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8da4d-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8da4d-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="8da4d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8da4d-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8da4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8da4d-114">Not supported.</span></span>|
|<span data-ttu-id="8da4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8da4d-115">Application</span></span>| <span data-ttu-id="8da4d-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8da4d-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8da4d-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="8da4d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8da4d-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8da4d-118">Global administrator</span></span>
* <span data-ttu-id="8da4d-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="8da4d-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8da4d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8da4d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="8da4d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8da4d-121">Request headers</span></span>

|<span data-ttu-id="8da4d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8da4d-122">Name</span></span>|<span data-ttu-id="8da4d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8da4d-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8da4d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8da4d-124">Authorization</span></span>|<span data-ttu-id="8da4d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8da4d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8da4d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8da4d-127">Request body</span></span>

<span data-ttu-id="8da4d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8da4d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8da4d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da4d-129">Response</span></span>

<span data-ttu-id="8da4d-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [идентитипровидерс](../resources/identityprovider.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8da4d-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8da4d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8da4d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8da4d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8da4d-132">Request</span></span>

<span data-ttu-id="8da4d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8da4d-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8da4d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8da4d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="8da4d-135">C#</span><span class="sxs-lookup"><span data-stu-id="8da4d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8da4d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8da4d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8da4d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8da4d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8da4d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da4d-138">Response</span></span>

<span data-ttu-id="8da4d-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8da4d-139">The following is an example of the response.</span></span>

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


