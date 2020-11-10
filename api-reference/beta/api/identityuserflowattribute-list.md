---
title: Список Идентитюсерфловаттрибутес
description: Получение списка объектов Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b22fa576d6aa918bf6b61ab05a75b2f103a89b02
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953158"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="d6830-103">Список Идентитюсерфловаттрибутес</span><span class="sxs-lookup"><span data-stu-id="d6830-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="d6830-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6830-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6830-105">Получение списка объектов [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="d6830-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6830-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6830-106">Permissions</span></span>

<span data-ttu-id="d6830-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6830-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6830-109">Permission type</span></span>      | <span data-ttu-id="d6830-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6830-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6830-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6830-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6830-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d6830-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="d6830-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6830-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d6830-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6830-114">Not supported.</span></span>|
|<span data-ttu-id="d6830-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6830-115">Application</span></span>|<span data-ttu-id="d6830-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d6830-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d6830-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d6830-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d6830-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d6830-118">Global administrator</span></span>
* <span data-ttu-id="d6830-119">Администратор атрибутов пользовательского процесса внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="d6830-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d6830-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6830-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="d6830-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6830-121">Request headers</span></span>

|<span data-ttu-id="d6830-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d6830-122">Name</span></span>|<span data-ttu-id="d6830-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d6830-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d6830-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6830-124">Authorization</span></span>|<span data-ttu-id="d6830-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6830-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6830-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6830-127">Request body</span></span>

<span data-ttu-id="d6830-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6830-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6830-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6830-129">Response</span></span>

<span data-ttu-id="d6830-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md)  в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6830-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6830-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d6830-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6830-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6830-132">Request</span></span>

<span data-ttu-id="d6830-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6830-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6830-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6830-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes
```
# <a name="c"></a>[<span data-ttu-id="d6830-135">C#</span><span class="sxs-lookup"><span data-stu-id="d6830-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6830-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6830-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6830-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6830-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6830-138">Java</span><span class="sxs-lookup"><span data-stu-id="d6830-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6830-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6830-139">Response</span></span>

<span data-ttu-id="d6830-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6830-140">The following is an example of the response.</span></span>

<span data-ttu-id="d6830-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d6830-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#userFlowAttributes",
    "value": [
      {
          "id": "City",
          "displayName": "City",
          "description": "Your city",
          "userFlowAttributeType": "builtIn",
          "dataType": "string"
      },
      {
          "id": "extension_d09380e2b4c6429a203fb816a04a7ad_Hobby",
          "displayName": "Hobby",
          "description": "Your hobby",
          "userFlowAttributeType": "custom",
          "dataType": "string",
      },
    ]
}
```
