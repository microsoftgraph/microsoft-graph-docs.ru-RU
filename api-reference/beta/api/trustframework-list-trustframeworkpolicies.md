---
title: Список ТрустфрамеворкполиЦиес
description: Эта операция перечисляет все объекты Трустфрамеворкполици в клиенте Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c28df77c6976deeb8a8bdf80adf7c4375ddb8d4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270576"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="f5d8f-103">Список ТрустфрамеворкполиЦиес</span><span class="sxs-lookup"><span data-stu-id="f5d8f-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="f5d8f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5d8f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5d8f-106">Получение списка [трустфрамеворкполиЦиес](../resources/trustframeworkpolicy.md) в клиенте или каталоге.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5d8f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5d8f-107">Permissions</span></span>

<span data-ttu-id="f5d8f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5d8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5d8f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5d8f-110">Permission type</span></span>      | <span data-ttu-id="f5d8f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5d8f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5d8f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5d8f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5d8f-113">Policy. Read. Трустфрамеворк, Policy. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f5d8f-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="f5d8f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5d8f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f5d8f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-115">Not supported.</span></span>|
|<span data-ttu-id="f5d8f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5d8f-116">Application</span></span>|<span data-ttu-id="f5d8f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-117">Not supported.</span></span>|

<span data-ttu-id="f5d8f-118">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f5d8f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5d8f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5d8f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f5d8f-120">Optional query parameters</span></span>

<span data-ttu-id="f5d8f-121">Этот метод поддерживает `$select` `$expand` [параметры запросов OData](/graph/query-parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5d8f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5d8f-122">Request headers</span></span>

|<span data-ttu-id="f5d8f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f5d8f-123">Name</span></span>|<span data-ttu-id="f5d8f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f5d8f-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f5d8f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5d8f-125">Authorization</span></span>|<span data-ttu-id="f5d8f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5d8f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f5d8f-128">Request body</span></span>

<span data-ttu-id="f5d8f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5d8f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5d8f-130">Response</span></span>

<span data-ttu-id="f5d8f-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ТРУСТФРАМЕВОРКПОЛИЦИ](../resources/trustframeworkpolicy.md) в представлении JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5d8f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f5d8f-132">Example</span></span>

<span data-ttu-id="f5d8f-133">В следующем примере показано получение всех **трустфрамеворкполиЦиес**.</span><span class="sxs-lookup"><span data-stu-id="f5d8f-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="f5d8f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5d8f-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```

##### <a name="response"></a><span data-ttu-id="f5d8f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5d8f-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "B2C_1A_CustomPolicy2"
        },
        {
            "id": "B2C_1A_CustomPolicy3"
        },
        {
            "id": "B2C_1A_SocialAndLocalAccounts_Base"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f5d8f-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f5d8f-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f5d8f-137">C#</span><span class="sxs-lookup"><span data-stu-id="f5d8f-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5d8f-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="f5d8f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f5d8f-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f5d8f-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
