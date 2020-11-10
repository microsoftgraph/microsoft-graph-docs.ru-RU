---
title: Получение Континуаусакцессевалуатионполици
description: Чтение свойств объекта Континуаусакцессевалуатионполици.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ba9d161e6c11863f20ab221e5e67ea6a5b7676c7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956957"
---
# <a name="get-continuousaccessevaluationpolicy"></a><span data-ttu-id="472f0-103">Получение Континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="472f0-103">Get continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="472f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="472f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="472f0-105">Чтение свойств и связей объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="472f0-105">Read the properties and relationships of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="472f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="472f0-106">Permissions</span></span>
<span data-ttu-id="472f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="472f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="472f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="472f0-109">Permission type</span></span>|<span data-ttu-id="472f0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="472f0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="472f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="472f0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="472f0-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="472f0-112">Policy.Read.All</span></span> |
|<span data-ttu-id="472f0-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="472f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="472f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="472f0-114">Not supported.</span></span> |
|<span data-ttu-id="472f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="472f0-115">Application</span></span>                            | <span data-ttu-id="472f0-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="472f0-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="472f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="472f0-117">HTTP request</span></span>

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="472f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="472f0-118">Optional query parameters</span></span>
<span data-ttu-id="472f0-119">Этот метод поддерживает параметр запроса OData "$select" для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="472f0-119">This method supports the '$select' OData query parameter to help customize the response.</span></span> <span data-ttu-id="472f0-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="472f0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="472f0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="472f0-121">Request headers</span></span>
|<span data-ttu-id="472f0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="472f0-122">Name</span></span>|<span data-ttu-id="472f0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="472f0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="472f0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="472f0-124">Authorization</span></span>|<span data-ttu-id="472f0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="472f0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="472f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="472f0-127">Request body</span></span>
<span data-ttu-id="472f0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="472f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="472f0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="472f0-129">Response</span></span>

<span data-ttu-id="472f0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="472f0-130">If successful, this method returns a `200 OK` response code and a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="472f0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="472f0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="472f0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="472f0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="472f0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="472f0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```
# <a name="c"></a>[<span data-ttu-id="472f0-134">C#</span><span class="sxs-lookup"><span data-stu-id="472f0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="472f0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="472f0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="472f0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="472f0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="472f0-137">Java</span><span class="sxs-lookup"><span data-stu-id="472f0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-continuousaccessevaluationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="472f0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="472f0-138">Response</span></span>

<span data-ttu-id="472f0-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="472f0-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
