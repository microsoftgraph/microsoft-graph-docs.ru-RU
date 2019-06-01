---
title: 'orgContact: получение менеджера'
description: Получение руководителя контакта
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93731249a3205bfa2730d6b5a259a371a3343da3
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657268"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="70f98-103">orgContact: получение менеджера</span><span class="sxs-lookup"><span data-stu-id="70f98-103">orgContact: Get manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70f98-104">Получение руководителя контакта</span><span class="sxs-lookup"><span data-stu-id="70f98-104">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="70f98-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70f98-105">Permissions</span></span>
<span data-ttu-id="70f98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70f98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70f98-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70f98-108">Permission type</span></span>      | <span data-ttu-id="70f98-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70f98-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70f98-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70f98-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70f98-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70f98-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70f98-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70f98-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70f98-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70f98-113">Not supported.</span></span>    |
|<span data-ttu-id="70f98-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70f98-114">Application</span></span> | <span data-ttu-id="70f98-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70f98-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70f98-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70f98-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70f98-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70f98-117">Optional query parameters</span></span>
<span data-ttu-id="70f98-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70f98-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70f98-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70f98-119">Request headers</span></span>
| <span data-ttu-id="70f98-120">Имя</span><span class="sxs-lookup"><span data-stu-id="70f98-120">Name</span></span>       | <span data-ttu-id="70f98-121">Тип</span><span class="sxs-lookup"><span data-stu-id="70f98-121">Type</span></span> | <span data-ttu-id="70f98-122">Описание</span><span class="sxs-lookup"><span data-stu-id="70f98-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70f98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70f98-123">Authorization</span></span>  | <span data-ttu-id="70f98-124">string</span><span class="sxs-lookup"><span data-stu-id="70f98-124">string</span></span>  | <span data-ttu-id="70f98-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70f98-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70f98-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70f98-127">Request body</span></span>
<span data-ttu-id="70f98-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70f98-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70f98-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="70f98-129">Response</span></span>

<span data-ttu-id="70f98-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70f98-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70f98-131">Пример</span><span class="sxs-lookup"><span data-stu-id="70f98-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="70f98-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="70f98-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="70f98-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="70f98-133">Response</span></span>

<span data-ttu-id="70f98-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70f98-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="70f98-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="70f98-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="70f98-137">C#</span><span class="sxs-lookup"><span data-stu-id="70f98-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_manager-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70f98-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="70f98-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_manager-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-get-manager.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-get-manager.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
