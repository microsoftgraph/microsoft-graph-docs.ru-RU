---
title: Список userflowidentityproviders
description: Список всех identityProviders в b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 5403bd03c06322bf91895609db601f2ccda4da9b
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439606"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="19fcb-103">Список userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="19fcb-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="19fcb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19fcb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19fcb-105">Получите поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="19fcb-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19fcb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19fcb-106">Permissions</span></span>

<span data-ttu-id="19fcb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19fcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19fcb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19fcb-109">Permission type</span></span>      | <span data-ttu-id="19fcb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19fcb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19fcb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19fcb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19fcb-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fcb-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="19fcb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19fcb-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="19fcb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fcb-114">Not supported.</span></span>|
|<span data-ttu-id="19fcb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="19fcb-115">Application</span></span>| <span data-ttu-id="19fcb-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fcb-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="19fcb-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="19fcb-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="19fcb-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="19fcb-118">Global administrator</span></span>
* <span data-ttu-id="19fcb-119">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="19fcb-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="19fcb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19fcb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="19fcb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19fcb-121">Request headers</span></span>

|<span data-ttu-id="19fcb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="19fcb-122">Name</span></span>|<span data-ttu-id="19fcb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="19fcb-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="19fcb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19fcb-124">Authorization</span></span>|<span data-ttu-id="19fcb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19fcb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19fcb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19fcb-127">Request body</span></span>

<span data-ttu-id="19fcb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19fcb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19fcb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="19fcb-129">Response</span></span>

<span data-ttu-id="19fcb-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityproviderbase.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="19fcb-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19fcb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="19fcb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="19fcb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="19fcb-132">Request</span></span>

<span data-ttu-id="19fcb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19fcb-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="19fcb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="19fcb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_userflowIdentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders
```
# <a name="c"></a>[<span data-ttu-id="19fcb-135">C#</span><span class="sxs-lookup"><span data-stu-id="19fcb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19fcb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19fcb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19fcb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19fcb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19fcb-138">Java</span><span class="sxs-lookup"><span data-stu-id="19fcb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflow-list-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="19fcb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="19fcb-139">Response</span></span>

<span data-ttu-id="19fcb-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="19fcb-140">The following is an example of the response.</span></span>

<span data-ttu-id="19fcb-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="19fcb-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.identityProviderBase)",
    "value": [
  {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "AADSignup-OAUTH",
            "displayName": "Azure Active Directory Sign up",
            "identityProviderType": "AADSignup"
        },
        {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "MSASignup-OAUTH",
            "displayName": "Microsoft Account (Preview)",
            "identityProviderType": "MicrosoftAccount"
        },
        {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "EmailOtpSignup-OAUTH",
            "displayName": "Email one-time passcode (Preview)",
            "identityProviderType": "EmailOTP"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Facebook-OAUTH",
            "displayName": "Facebook",
            "identityProviderType": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}

```
