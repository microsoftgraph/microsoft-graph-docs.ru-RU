---
title: Список Идентитюсерфловаттрибутес
description: Получение списка объектов Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39536cd2a8e9a2f5c1ad928384e31dcee1e7672a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904059"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="c01ff-103">Список Идентитюсерфловаттрибутес</span><span class="sxs-lookup"><span data-stu-id="c01ff-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="c01ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c01ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c01ff-105">Получение списка объектов [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="c01ff-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c01ff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c01ff-106">Permissions</span></span>

<span data-ttu-id="c01ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c01ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c01ff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c01ff-109">Permission type</span></span>      | <span data-ttu-id="c01ff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c01ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c01ff-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c01ff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c01ff-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c01ff-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="c01ff-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c01ff-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c01ff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c01ff-114">Not supported.</span></span>|
|<span data-ttu-id="c01ff-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c01ff-115">Application</span></span>|<span data-ttu-id="c01ff-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c01ff-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c01ff-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="c01ff-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c01ff-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c01ff-118">Global administrator</span></span>
* <span data-ttu-id="c01ff-119">Администратор атрибутов пользовательского процесса внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="c01ff-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c01ff-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c01ff-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="c01ff-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c01ff-121">Request headers</span></span>

|<span data-ttu-id="c01ff-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c01ff-122">Name</span></span>|<span data-ttu-id="c01ff-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c01ff-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c01ff-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c01ff-124">Authorization</span></span>|<span data-ttu-id="c01ff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c01ff-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c01ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c01ff-127">Request body</span></span>

<span data-ttu-id="c01ff-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c01ff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c01ff-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c01ff-129">Response</span></span>

<span data-ttu-id="c01ff-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md)  в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c01ff-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c01ff-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c01ff-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c01ff-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c01ff-132">Request</span></span>

<span data-ttu-id="c01ff-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c01ff-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c01ff-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c01ff-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes
```
# <a name="c"></a>[<span data-ttu-id="c01ff-135">C#</span><span class="sxs-lookup"><span data-stu-id="c01ff-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c01ff-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c01ff-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c01ff-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c01ff-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c01ff-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c01ff-138">Response</span></span>

<span data-ttu-id="c01ff-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c01ff-139">The following is an example of the response.</span></span>

<span data-ttu-id="c01ff-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c01ff-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
