---
title: Список всех identityProviders в b2xIdentityUserFlow (обесценив)
description: Список всех identityProviders в b2xIdentityUserFlow (обесценив).
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 28265310a7dd0ff111babb89f218797ba194e03f
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400931"
---
# <a name="list-all-identityproviders-in-a-b2xidentityuserflow-deprecated"></a><span data-ttu-id="e9833-103">Список всех identityProviders в b2xIdentityUserFlow (обесценив)</span><span class="sxs-lookup"><span data-stu-id="e9833-103">List all identityProviders in a b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="e9833-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9833-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="e9833-105">Получите поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="e9833-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9833-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9833-106">Permissions</span></span>

<span data-ttu-id="e9833-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9833-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9833-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9833-109">Permission type</span></span>      | <span data-ttu-id="e9833-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9833-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9833-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9833-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9833-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9833-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e9833-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9833-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e9833-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9833-114">Not supported.</span></span>|
|<span data-ttu-id="e9833-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e9833-115">Application</span></span>| <span data-ttu-id="e9833-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9833-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e9833-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="e9833-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e9833-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e9833-118">Global administrator</span></span>
* <span data-ttu-id="e9833-119">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="e9833-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e9833-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9833-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="e9833-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9833-121">Request headers</span></span>

|<span data-ttu-id="e9833-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e9833-122">Name</span></span>|<span data-ttu-id="e9833-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e9833-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e9833-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9833-124">Authorization</span></span>|<span data-ttu-id="e9833-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9833-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9833-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9833-127">Request body</span></span>

<span data-ttu-id="e9833-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9833-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9833-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9833-129">Response</span></span>

<span data-ttu-id="e9833-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e9833-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9833-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e9833-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9833-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9833-132">Request</span></span>

<span data-ttu-id="e9833-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9833-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```

### <a name="response"></a><span data-ttu-id="e9833-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9833-134">Response</span></span>

<span data-ttu-id="e9833-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e9833-135">The following is an example of the response.</span></span>

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
