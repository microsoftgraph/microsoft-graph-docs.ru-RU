---
title: Список userflowidentityproviders
description: Список всех identityProviders в b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 63bf686abbe51a9abd132e71d1e4472fc45c0849
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401179"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="0ceb1-103">Список userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="0ceb1-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="0ceb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ceb1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ceb1-105">Получите поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb1-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ceb1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ceb1-106">Permissions</span></span>

<span data-ttu-id="0ceb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ceb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ceb1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ceb1-109">Permission type</span></span>      | <span data-ttu-id="0ceb1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ceb1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ceb1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ceb1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ceb1-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ceb1-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0ceb1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ceb1-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0ceb1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-114">Not supported.</span></span>|
|<span data-ttu-id="0ceb1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ceb1-115">Application</span></span>| <span data-ttu-id="0ceb1-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ceb1-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0ceb1-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="0ceb1-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0ceb1-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0ceb1-118">Global administrator</span></span>
* <span data-ttu-id="0ceb1-119">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="0ceb1-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0ceb1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ceb1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="0ceb1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ceb1-121">Request headers</span></span>

|<span data-ttu-id="0ceb1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0ceb1-122">Name</span></span>|<span data-ttu-id="0ceb1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0ceb1-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0ceb1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ceb1-124">Authorization</span></span>|<span data-ttu-id="0ceb1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ceb1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ceb1-127">Request body</span></span>

<span data-ttu-id="0ceb1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ceb1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ceb1-129">Response</span></span>

<span data-ttu-id="0ceb1-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityproviderbase.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ceb1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0ceb1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ceb1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ceb1-132">Request</span></span>

<span data-ttu-id="0ceb1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_userflowIdentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders
```

### <a name="response"></a><span data-ttu-id="0ceb1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ceb1-134">Response</span></span>

<span data-ttu-id="0ceb1-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-135">The following is an example of the response.</span></span>

<span data-ttu-id="0ceb1-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
