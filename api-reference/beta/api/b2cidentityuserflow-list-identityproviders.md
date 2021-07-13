---
title: Список всех identityProviders в b2cIdentityUserFlow (обесценив)
description: Список всех identityProviders в b2cIdentityUserFlow. (неоконт.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7e83384f009c273197ea8bd8b978e27dd75263a8
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400980"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="f3476-104">Список всех identityProviders в b2cIdentityUserFlow (обесценив)</span><span class="sxs-lookup"><span data-stu-id="f3476-104">List all identityProviders in a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="f3476-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3476-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="f3476-106">Получите поставщиков удостоверений в [объекте b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f3476-106">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3476-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3476-107">Permissions</span></span>

<span data-ttu-id="f3476-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3476-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3476-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3476-110">Permission type</span></span>      | <span data-ttu-id="f3476-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3476-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3476-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3476-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3476-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3476-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f3476-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3476-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f3476-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3476-115">Not supported.</span></span>|
|<span data-ttu-id="f3476-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3476-116">Application</span></span>| <span data-ttu-id="f3476-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3476-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f3476-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f3476-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f3476-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f3476-119">Global administrator</span></span>
* <span data-ttu-id="f3476-120">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="f3476-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f3476-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3476-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="f3476-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3476-122">Request headers</span></span>

|<span data-ttu-id="f3476-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f3476-123">Name</span></span>|<span data-ttu-id="f3476-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f3476-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f3476-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3476-125">Authorization</span></span>|<span data-ttu-id="f3476-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3476-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3476-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3476-128">Request body</span></span>

<span data-ttu-id="f3476-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3476-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3476-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3476-130">Response</span></span>

<span data-ttu-id="f3476-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f3476-131">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3476-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f3476-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3476-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3476-133">Request</span></span>

<span data-ttu-id="f3476-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3476-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```

### <a name="response"></a><span data-ttu-id="f3476-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3476-135">Response</span></span>

<span data-ttu-id="f3476-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f3476-136">The following is an example of the response.</span></span>

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
