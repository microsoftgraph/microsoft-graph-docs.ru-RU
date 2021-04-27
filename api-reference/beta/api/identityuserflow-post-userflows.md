---
title: Создание пользовательского потока
description: Используйте этот API для создания нового пользовательского потока.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e05529179ce498d58857a0308fcd615866cf39ed
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040674"
---
# <a name="create-userflow"></a><span data-ttu-id="37d3b-103">Создание пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="37d3b-103">Create userFlow</span></span>

<span data-ttu-id="37d3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37d3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37d3b-105">Создание нового [объекта пользовательского потока.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="37d3b-105">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37d3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37d3b-106">Permissions</span></span>

<span data-ttu-id="37d3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37d3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37d3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37d3b-109">Permission type</span></span>                        | <span data-ttu-id="37d3b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37d3b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37d3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37d3b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37d3b-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d3b-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="37d3b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37d3b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37d3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d3b-114">Not supported.</span></span> |
| <span data-ttu-id="37d3b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37d3b-115">Application</span></span>                            | <span data-ttu-id="37d3b-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d3b-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37d3b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37d3b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="37d3b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37d3b-118">Request headers</span></span>

| <span data-ttu-id="37d3b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="37d3b-119">Name</span></span>          | <span data-ttu-id="37d3b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="37d3b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="37d3b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37d3b-121">Authorization</span></span> | <span data-ttu-id="37d3b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37d3b-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="37d3b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37d3b-124">Content-type</span></span> | <span data-ttu-id="37d3b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37d3b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37d3b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37d3b-127">Request body</span></span>

<span data-ttu-id="37d3b-128">В теле запроса поставляем JSON-представление [объекта userFlow.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="37d3b-128">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="37d3b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="37d3b-129">Response</span></span>

<span data-ttu-id="37d3b-130">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект пользовательского потока](../resources/identityuserflow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="37d3b-130">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37d3b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="37d3b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37d3b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="37d3b-132">Request</span></span>

<span data-ttu-id="37d3b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37d3b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37d3b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="37d3b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_identitycontainer"
}-->

```http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json

{
  "id": "Pol1",
  "userFlowType": "signUpOrSignIn",
  "userFlowTypeVersion": 1
}
```
# <a name="c"></a>[<span data-ttu-id="37d3b-135">C#</span><span class="sxs-lookup"><span data-stu-id="37d3b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37d3b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37d3b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37d3b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37d3b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37d3b-138">Java</span><span class="sxs-lookup"><span data-stu-id="37d3b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflow-from-identitycontainer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37d3b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="37d3b-139">Response</span></span>

<span data-ttu-id="37d3b-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="37d3b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="37d3b-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37d3b-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_identityuserflow_from_identitycontainer/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


