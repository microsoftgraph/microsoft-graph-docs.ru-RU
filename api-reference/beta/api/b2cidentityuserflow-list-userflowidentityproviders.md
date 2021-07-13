---
title: Список userflowidentityproviders
description: Список всех поставщиков удостоверений в b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 618d9c0c1c7a27e015e45192f72b8c1455e0522c
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401183"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="c7fbb-103">Список userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="c7fbb-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="c7fbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7fbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7fbb-105">Получите поставщиков удостоверений в [объекте b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="c7fbb-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7fbb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7fbb-106">Permissions</span></span>

<span data-ttu-id="c7fbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7fbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7fbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7fbb-109">Permission type</span></span>      | <span data-ttu-id="c7fbb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7fbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7fbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7fbb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7fbb-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7fbb-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c7fbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7fbb-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c7fbb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7fbb-114">Not supported.</span></span>|
|<span data-ttu-id="c7fbb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c7fbb-115">Application</span></span>| <span data-ttu-id="c7fbb-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7fbb-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c7fbb-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="c7fbb-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c7fbb-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c7fbb-118">Global administrator</span></span>
* <span data-ttu-id="c7fbb-119">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="c7fbb-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c7fbb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7fbb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="c7fbb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7fbb-121">Request headers</span></span>

|<span data-ttu-id="c7fbb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c7fbb-122">Name</span></span>|<span data-ttu-id="c7fbb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c7fbb-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c7fbb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7fbb-124">Authorization</span></span>|<span data-ttu-id="c7fbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7fbb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7fbb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7fbb-127">Request body</span></span>

<span data-ttu-id="c7fbb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7fbb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7fbb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7fbb-129">Response</span></span>

<span data-ttu-id="c7fbb-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityproviderbase.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c7fbb-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7fbb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c7fbb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7fbb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7fbb-132">Request</span></span>

<span data-ttu-id="c7fbb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7fbb-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_userflowidentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders
```

### <a name="response"></a><span data-ttu-id="c7fbb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7fbb-134">Response</span></span>

<span data-ttu-id="c7fbb-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c7fbb-135">The following is an example of the response.</span></span>
><span data-ttu-id="c7fbb-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7fbb-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
            "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
            "id": "OIDC-V1-AD_Test-3e393390-ed2d-4794-97f6-5c1a1ccc61f7",
            "displayName": "OIDC AD Test",
            "clientId": "fe1b1576-adca-4bef-b321-076fde19950b",
            "clientSecret": "******",
            "scope": "openid",
            "metadataUrl": "https://login.microsoftonline.com/contoso.com/.well-known/openid-configuration",
            "domainHint": "",
            "responseType": "code",
            "responseMode": "form_post",
            "claimsMapping": {
                "userId": "oid",
                "displayName": "samuel",
                "givenName": "samuel",
                "surname": "emmense",
                "email": "sam.e@contoso.com"
            }
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Apple-Managed-OIDC",
            "displayName": "Sign in with Apple",
            "identityProviderType": "AppleManaged",
            "clientId": "com.contoso.client",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "MSA-OIDC",
            "displayName": "Microsoft Account",
            "identityProviderType": "Microsoft",
            "clientId": "1e02ac8a-0c37-4046-abe4-35098a840090",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Facebook-OAUTH",
            "displayName": "Facebook",
            "identityProviderType": "Facebook",
            "clientId": "576628889930009",
            "clientSecret": "******"
        }
    ]
}
```
