---
title: Перечисление объектов secureScores
description: Получение списка объектов Секурескоре.
author: preetikr
localization_priority: Normal
ms.openlocfilehash: 9cc407da1a4a511ec309b50607ddaac33fe28a27
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951330"
---
# <a name="list-securescores"></a><span data-ttu-id="10c60-103">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="10c60-103">List secureScores</span></span>

<span data-ttu-id="10c60-104">Получение списка объектов [секурескоре](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="10c60-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="10c60-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10c60-105">Permissions</span></span>

<span data-ttu-id="10c60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10c60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10c60-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10c60-108">Permission type</span></span>      | <span data-ttu-id="10c60-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10c60-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10c60-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10c60-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="10c60-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="10c60-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="10c60-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10c60-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="10c60-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10c60-113">Not supported.</span></span>  |
|<span data-ttu-id="10c60-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10c60-114">Application</span></span> | <span data-ttu-id="10c60-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="10c60-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10c60-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10c60-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10c60-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10c60-117">Optional query parameters</span></span>

<span data-ttu-id="10c60-118">Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="10c60-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="10c60-119">`$top` возвращает объединенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="10c60-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="10c60-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10c60-120">Request headers</span></span>

| <span data-ttu-id="10c60-121">Имя</span><span class="sxs-lookup"><span data-stu-id="10c60-121">Name</span></span>      |<span data-ttu-id="10c60-122">Описание</span><span class="sxs-lookup"><span data-stu-id="10c60-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10c60-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10c60-123">Authorization</span></span>  | <span data-ttu-id="10c60-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="10c60-124">Bearer {code}.</span></span> <span data-ttu-id="10c60-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="10c60-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10c60-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10c60-126">Request body</span></span>

<span data-ttu-id="10c60-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10c60-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="10c60-128">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="10c60-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="10c60-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="10c60-129">Response</span></span>

<span data-ttu-id="10c60-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **секурескорес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10c60-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10c60-131">Пример</span><span class="sxs-lookup"><span data-stu-id="10c60-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="10c60-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="10c60-132">Request</span></span>

<span data-ttu-id="10c60-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10c60-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="10c60-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="10c60-134">Response</span></span>

<span data-ttu-id="10c60-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10c60-135">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="10c60-136">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="10c60-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="10c60-137">C#</span><span class="sxs-lookup"><span data-stu-id="10c60-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securescores-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10c60-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="10c60-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securescores-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
