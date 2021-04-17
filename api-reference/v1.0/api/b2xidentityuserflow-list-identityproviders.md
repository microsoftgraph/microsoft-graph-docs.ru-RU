---
title: Перечисление объектов identityProvider
description: Список всех identityProviders в b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 01e1e3092c31d3bc9cef921e817da991e9b804cb
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883374"
---
# <a name="list-identityproviders"></a><span data-ttu-id="39f74-103">Перечисление объектов identityProvider</span><span class="sxs-lookup"><span data-stu-id="39f74-103">List identityProviders</span></span>

<span data-ttu-id="39f74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39f74-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39f74-105">Получите поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="39f74-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39f74-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39f74-106">Permissions</span></span>

<span data-ttu-id="39f74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39f74-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39f74-109">Permission type</span></span>      | <span data-ttu-id="39f74-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39f74-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39f74-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39f74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39f74-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39f74-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="39f74-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39f74-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="39f74-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39f74-114">Not supported.</span></span>|
|<span data-ttu-id="39f74-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39f74-115">Application</span></span>| <span data-ttu-id="39f74-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39f74-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="39f74-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="39f74-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="39f74-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="39f74-118">Global administrator</span></span>
* <span data-ttu-id="39f74-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="39f74-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="39f74-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39f74-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="39f74-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39f74-121">Request headers</span></span>

|<span data-ttu-id="39f74-122">Имя</span><span class="sxs-lookup"><span data-stu-id="39f74-122">Name</span></span>|<span data-ttu-id="39f74-123">Описание</span><span class="sxs-lookup"><span data-stu-id="39f74-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="39f74-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39f74-124">Authorization</span></span>|<span data-ttu-id="39f74-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39f74-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39f74-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39f74-127">Request body</span></span>

<span data-ttu-id="39f74-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39f74-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39f74-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="39f74-129">Response</span></span>

<span data-ttu-id="39f74-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="39f74-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39f74-131">Пример</span><span class="sxs-lookup"><span data-stu-id="39f74-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="39f74-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="39f74-132">Request</span></span>

<span data-ttu-id="39f74-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39f74-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/identityProviders
```

### <a name="response"></a><span data-ttu-id="39f74-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="39f74-134">Response</span></span>

<span data-ttu-id="39f74-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="39f74-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider",
  "isCollection": true
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
 "description": "get_b2xuserflow_list_identityproviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
