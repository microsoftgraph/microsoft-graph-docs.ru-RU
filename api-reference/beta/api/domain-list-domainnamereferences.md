---
title: Список Домаиннамереференцес
description: Получение списка directoryObject со ссылкой на домен. Возвращаемый список будет содержать все объекты каталога с зависимостью от домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f1854882ce78084bfda3f428a19e4bc4cd02d78c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589207"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="ea63f-104">Список Домаиннамереференцес</span><span class="sxs-lookup"><span data-stu-id="ea63f-104">List domainNameReferences</span></span>

<span data-ttu-id="ea63f-105">Получение списка [directoryObject](../resources/directoryobject.md) со ссылкой на домен.</span><span class="sxs-lookup"><span data-stu-id="ea63f-105">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="ea63f-106">Возвращаемый список будет содержать все объекты каталога с зависимостью от домена.</span><span class="sxs-lookup"><span data-stu-id="ea63f-106">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea63f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea63f-107">Permissions</span></span>

<span data-ttu-id="ea63f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea63f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ea63f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea63f-110">Permission type</span></span>      | <span data-ttu-id="ea63f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea63f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea63f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea63f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ea63f-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea63f-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="ea63f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea63f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea63f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea63f-115">Not supported.</span></span>    |
|<span data-ttu-id="ea63f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea63f-116">Application</span></span> | <span data-ttu-id="ea63f-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea63f-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea63f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea63f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="ea63f-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="ea63f-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ea63f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea63f-120">Optional query parameters</span></span>

<span data-ttu-id="ea63f-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea63f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea63f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea63f-122">Request headers</span></span>

| <span data-ttu-id="ea63f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ea63f-123">Name</span></span>      |<span data-ttu-id="ea63f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ea63f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea63f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea63f-125">Authorization</span></span>  | <span data-ttu-id="ea63f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea63f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea63f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea63f-128">Request body</span></span>

<span data-ttu-id="ea63f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea63f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea63f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea63f-130">Response</span></span>

<span data-ttu-id="ea63f-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea63f-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea63f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ea63f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea63f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea63f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="ea63f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea63f-134">Response</span></span>
<span data-ttu-id="ea63f-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea63f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ea63f-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ea63f-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ea63f-138">Языках</span><span class="sxs-lookup"><span data-stu-id="ea63f-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ea63f-139">Язык</span><span class="sxs-lookup"><span data-stu-id="ea63f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
