---
title: Список ТрустфрамеворкполиЦиес
description: Эта операция перечисляет все объекты Трустфрамеворкполици в клиенте Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32b6314409bd9253e85d8a9df31cf005d0fe3983
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734474"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="d7207-103">Список ТрустфрамеворкполиЦиес</span><span class="sxs-lookup"><span data-stu-id="d7207-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="d7207-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7207-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7207-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7207-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7207-106">Получение списка [трустфрамеворкполиЦиес](../resources/trustframeworkpolicy.md) в клиенте или каталоге.</span><span class="sxs-lookup"><span data-stu-id="d7207-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7207-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7207-107">Permissions</span></span>

<span data-ttu-id="d7207-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7207-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7207-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7207-110">Permission type</span></span>      | <span data-ttu-id="d7207-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7207-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7207-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7207-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7207-113">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7207-113">Policy.Read.All</span></span>|
|<span data-ttu-id="d7207-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7207-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d7207-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7207-115">Not supported.</span></span>|
|<span data-ttu-id="d7207-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7207-116">Application</span></span>|<span data-ttu-id="d7207-117">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7207-117">Policy.Read.All</span></span>|

<span data-ttu-id="d7207-118">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="d7207-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d7207-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7207-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7207-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7207-120">Optional query parameters</span></span>

<span data-ttu-id="d7207-121">Этот метод поддерживает `$select` `$expand` [параметры запросов OData](/graph/query-parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d7207-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7207-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7207-122">Request headers</span></span>

|<span data-ttu-id="d7207-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d7207-123">Name</span></span>|<span data-ttu-id="d7207-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d7207-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d7207-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7207-125">Authorization</span></span>|<span data-ttu-id="d7207-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7207-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7207-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7207-128">Request body</span></span>

<span data-ttu-id="d7207-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7207-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7207-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7207-130">Response</span></span>

<span data-ttu-id="d7207-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ТРУСТФРАМЕВОРКПОЛИЦИ](../resources/trustframeworkpolicy.md) в представлении JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7207-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7207-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d7207-132">Example</span></span>

<span data-ttu-id="d7207-133">В следующем примере показано получение всех **трустфрамеворкполиЦиес**.</span><span class="sxs-lookup"><span data-stu-id="d7207-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="d7207-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7207-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d7207-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7207-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7207-136">C#</span><span class="sxs-lookup"><span data-stu-id="d7207-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7207-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7207-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7207-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7207-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d7207-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7207-139">Response</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
