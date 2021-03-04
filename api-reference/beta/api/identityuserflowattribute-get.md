---
title: Get identityUserFlowAttribute
description: Извлечение свойств и связей объекта identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: f98dc9a69aee1297d26ef4ed9891f9035a297ced
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435275"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="89e9f-103">Get identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="89e9f-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="89e9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89e9f-105">Извлечение свойств и связей [объекта identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="89e9f-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89e9f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89e9f-106">Permissions</span></span>

<span data-ttu-id="89e9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89e9f-109">Permission type</span></span>      | <span data-ttu-id="89e9f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89e9f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89e9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89e9f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89e9f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e9f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="89e9f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89e9f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="89e9f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89e9f-114">Not supported.</span></span>|
|<span data-ttu-id="89e9f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="89e9f-115">Application</span></span>|<span data-ttu-id="89e9f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e9f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="89e9f-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="89e9f-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="89e9f-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="89e9f-118">Global administrator</span></span>
* <span data-ttu-id="89e9f-119">Администратор атрибута потока внешних удостоверений</span><span class="sxs-lookup"><span data-stu-id="89e9f-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="89e9f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89e9f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="89e9f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89e9f-121">Request headers</span></span>

|<span data-ttu-id="89e9f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="89e9f-122">Name</span></span>|<span data-ttu-id="89e9f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="89e9f-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="89e9f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89e9f-124">Authorization</span></span>|<span data-ttu-id="89e9f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89e9f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89e9f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89e9f-127">Request body</span></span>

<span data-ttu-id="89e9f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89e9f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89e9f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="89e9f-129">Response</span></span>

<span data-ttu-id="89e9f-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON в тексте ответа [identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="89e9f-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89e9f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="89e9f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89e9f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="89e9f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="89e9f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="89e9f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="89e9f-134">C#</span><span class="sxs-lookup"><span data-stu-id="89e9f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89e9f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89e9f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89e9f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89e9f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89e9f-137">Java</span><span class="sxs-lookup"><span data-stu-id="89e9f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89e9f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="89e9f-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "City",
    "displayName": "City",
    "description": "Your city",
    "userFlowAttributeType": "builtIn",
    "dataType": "string"
}
```
