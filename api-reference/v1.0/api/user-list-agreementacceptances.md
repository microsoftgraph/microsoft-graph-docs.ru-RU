---
title: Перечисление agreementAcceptances
description: Извлечение списка объектов agreementAcceptance пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 40249bcddeb426269151d32ec842ca097a847e8c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777470"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="d934e-103">Перечисление agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="d934e-103">List agreementAcceptances</span></span>

<span data-ttu-id="d934e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d934e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d934e-105">Извлечение списка объектов [agreementAcceptance пользователя.](../resources/agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="d934e-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d934e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d934e-106">Permissions</span></span>
<span data-ttu-id="d934e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d934e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d934e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d934e-109">Permission type</span></span>                        | <span data-ttu-id="d934e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d934e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d934e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d934e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d934e-112">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="d934e-112">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="d934e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d934e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d934e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d934e-114">Not supported.</span></span> |
|<span data-ttu-id="d934e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d934e-115">Application</span></span>                            | <span data-ttu-id="d934e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d934e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d934e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d934e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/agreementAcceptances
GET /users/{id | userPrincipalName}/agreementAcceptances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d934e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d934e-118">Optional query parameters</span></span>
<span data-ttu-id="d934e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d934e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d934e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d934e-120">Request headers</span></span>
| <span data-ttu-id="d934e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d934e-121">Name</span></span>      |<span data-ttu-id="d934e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d934e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d934e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d934e-123">Authorization</span></span> | <span data-ttu-id="d934e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d934e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d934e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d934e-126">Request body</span></span>
<span data-ttu-id="d934e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d934e-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d934e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d934e-128">Response</span></span>
<span data-ttu-id="d934e-129">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов agreementAcceptance](../resources/agreementacceptance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d934e-129">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d934e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d934e-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="d934e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d934e-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d934e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d934e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/agreementAcceptances

GET https://graph.microsoft.com/v1.0/users/f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="d934e-133">C#</span><span class="sxs-lookup"><span data-stu-id="d934e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d934e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d934e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d934e-135">Java</span><span class="sxs-lookup"><span data-stu-id="d934e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d934e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d934e-136">Response</span></span>
><span data-ttu-id="d934e-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d934e-137">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "093b947f-8363-4979-a47d-4c52b33ee1be",
      "userId": "f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf",
      "agreementFileId": "f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf",
      "recordedDateTime": "2021-03-10T00:39:56.0523527Z",
      "userDisplayName": "Test_User",
      "userPrincipalName": "Test_User@TestTenant.onmicrosoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
