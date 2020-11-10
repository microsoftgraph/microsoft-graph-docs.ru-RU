---
title: Получение Идентитюсерфловаттрибуте
description: Получение свойств и связей объекта Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2497ac509376aa07b692ac8d137e64b5c299ab49
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953187"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="b3b78-103">Получение Идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="b3b78-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="b3b78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3b78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3b78-105">Получение свойств и связей объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="b3b78-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3b78-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3b78-106">Permissions</span></span>

<span data-ttu-id="b3b78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3b78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3b78-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3b78-109">Permission type</span></span>      | <span data-ttu-id="b3b78-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3b78-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3b78-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3b78-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3b78-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3b78-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="b3b78-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3b78-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b3b78-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3b78-114">Not supported.</span></span>|
|<span data-ttu-id="b3b78-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3b78-115">Application</span></span>|<span data-ttu-id="b3b78-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3b78-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="b3b78-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="b3b78-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b3b78-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b3b78-118">Global administrator</span></span>
* <span data-ttu-id="b3b78-119">Администратор атрибутов пользовательского процесса внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="b3b78-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b3b78-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3b78-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b3b78-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3b78-121">Request headers</span></span>

|<span data-ttu-id="b3b78-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b3b78-122">Name</span></span>|<span data-ttu-id="b3b78-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b3b78-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b3b78-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3b78-124">Authorization</span></span>|<span data-ttu-id="b3b78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3b78-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3b78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3b78-127">Request body</span></span>

<span data-ttu-id="b3b78-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3b78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3b78-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3b78-129">Response</span></span>

<span data-ttu-id="b3b78-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3b78-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3b78-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3b78-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3b78-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3b78-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b3b78-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3b78-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="b3b78-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3b78-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3b78-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3b78-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3b78-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3b78-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3b78-137">Java</span><span class="sxs-lookup"><span data-stu-id="b3b78-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3b78-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3b78-138">Response</span></span>

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
