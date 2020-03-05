---
title: Список ТрустфрамеворкполиЦиес
description: Эта операция перечисляет все объекты Трустфрамеворкполици в клиенте Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61e110d00bb39074314f847cdfb530b9488a855f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452185"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="e4a19-103">Список ТрустфрамеворкполиЦиес</span><span class="sxs-lookup"><span data-stu-id="e4a19-103">List trustFrameworkPolicies</span></span>

<span data-ttu-id="e4a19-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e4a19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4a19-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4a19-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4a19-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4a19-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4a19-107">Получение списка [трустфрамеворкполиЦиес](../resources/trustframeworkpolicy.md) в клиенте или каталоге.</span><span class="sxs-lookup"><span data-stu-id="e4a19-107">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a19-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4a19-108">Permissions</span></span>

<span data-ttu-id="e4a19-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4a19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4a19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4a19-111">Permission type</span></span>      | <span data-ttu-id="e4a19-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4a19-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4a19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4a19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4a19-114">Policy. Read. ALL, Policy. ReadWrite. Трустфрамеворк</span><span class="sxs-lookup"><span data-stu-id="e4a19-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="e4a19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4a19-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e4a19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4a19-116">Not supported.</span></span>|
|<span data-ttu-id="e4a19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4a19-117">Application</span></span>|<span data-ttu-id="e4a19-118">Policy. Read. ALL, Policy. ReadWrite. Трустфрамеворк</span><span class="sxs-lookup"><span data-stu-id="e4a19-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="e4a19-119">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="e4a19-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e4a19-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4a19-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4a19-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4a19-121">Optional query parameters</span></span>

<span data-ttu-id="e4a19-122">Этот метод поддерживает `$select` `$expand` [параметры запросов OData](/graph/query-parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e4a19-122">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4a19-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4a19-123">Request headers</span></span>

|<span data-ttu-id="e4a19-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e4a19-124">Name</span></span>|<span data-ttu-id="e4a19-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e4a19-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e4a19-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4a19-126">Authorization</span></span>|<span data-ttu-id="e4a19-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4a19-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4a19-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4a19-129">Request body</span></span>

<span data-ttu-id="e4a19-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4a19-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4a19-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4a19-131">Response</span></span>

<span data-ttu-id="e4a19-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ТРУСТФРАМЕВОРКПОЛИЦИ](../resources/trustframeworkpolicy.md) в представлении JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4a19-132">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4a19-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e4a19-133">Example</span></span>

<span data-ttu-id="e4a19-134">В следующем примере показано получение всех **трустфрамеворкполиЦиес**.</span><span class="sxs-lookup"><span data-stu-id="e4a19-134">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="e4a19-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4a19-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e4a19-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a19-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="c"></a>[<span data-ttu-id="e4a19-137">C#</span><span class="sxs-lookup"><span data-stu-id="e4a19-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4a19-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4a19-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4a19-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4a19-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4a19-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4a19-140">Response</span></span>

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
