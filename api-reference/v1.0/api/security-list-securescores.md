---
title: Перечисление объектов secureScores
description: Получение списка объектов Секурескоре.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 3eea4465c7cbaa767ff03684515431adbdb560a6
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330363"
---
# <a name="list-securescores"></a><span data-ttu-id="753a7-103">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="753a7-103">List secureScores</span></span>

<span data-ttu-id="753a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="753a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="753a7-105">Получение списка объектов [секурескоре](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="753a7-105">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="753a7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="753a7-106">Permissions</span></span>

<span data-ttu-id="753a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="753a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="753a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="753a7-109">Permission type</span></span>      | <span data-ttu-id="753a7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="753a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="753a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="753a7-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="753a7-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="753a7-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="753a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="753a7-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="753a7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="753a7-114">Not supported.</span></span>  |
|<span data-ttu-id="753a7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="753a7-115">Application</span></span> | <span data-ttu-id="753a7-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="753a7-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="753a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="753a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="753a7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="753a7-118">Optional query parameters</span></span>

<span data-ttu-id="753a7-119">Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="753a7-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="753a7-120">`$top` возвращает объединенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="753a7-120">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="753a7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="753a7-121">Request headers</span></span>

| <span data-ttu-id="753a7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="753a7-122">Name</span></span>      |<span data-ttu-id="753a7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="753a7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="753a7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="753a7-124">Authorization</span></span>  | <span data-ttu-id="753a7-125">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="753a7-125">Bearer {code}.</span></span> <span data-ttu-id="753a7-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="753a7-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="753a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="753a7-127">Request body</span></span>

<span data-ttu-id="753a7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="753a7-128">Do not supply a request body for this method.</span></span> <span data-ttu-id="753a7-129">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="753a7-129">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="753a7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="753a7-130">Response</span></span>

<span data-ttu-id="753a7-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **секурескорес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="753a7-131">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="753a7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="753a7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="753a7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="753a7-133">Request</span></span>

<span data-ttu-id="753a7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="753a7-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="753a7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="753a7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="c"></a>[<span data-ttu-id="753a7-136">C#</span><span class="sxs-lookup"><span data-stu-id="753a7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="753a7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="753a7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="753a7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="753a7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="753a7-139">Java</span><span class="sxs-lookup"><span data-stu-id="753a7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescores-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="753a7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="753a7-140">Response</span></span>

<span data-ttu-id="753a7-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="753a7-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScore",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "00000001-0001-0001-0001-000000000001c_2019-03-19",
            "azureTenantId": "00000001-0001-0001-0001-000000000001c",
            "activeUserCount": 0,
            "createdDateTime": "2019-03-19T15:21:00Z",
            "currentScore": 387.0,
            "enabledServices": [
                "HasExchange",
                "HasSharePoint",
                "HasInTune"
            ],
            "licensedUserCount": 100,
            "maxScore": 697.0,
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": 37.0
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": 46.0
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": 109.0
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "Identity",
                    "controlName": "AdminMFA",
                    "description": "Requiring multi-factor authentication (MFA) for all Azure Active Directory accounts with privileged roles",
                    "score": 35.0
                },
                {
                    "controlCategory": "Data",
                    "controlName": "DLPEnabled",
                    "description": "Data Loss Prevention (DLP) policies can be used to comply with business standards and industry regulations.",
                    "score": 20.0
                }
            ],
            "vendorInformation": {
                "provider": "SecureScore",
                "providerVersion": null,
                "subProvider": null,
                "vendor": "Microsoft"
            }
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

