---
title: Перечисление объектов secureScoreControlProfiles
description: Получение свойств и связей объекта Секурескореконтролпрофилес.
localization_priority: Normal
ms.openlocfilehash: 94f94feb5f540d3a830b97ec3defe7972b345557
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638818"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="8b4ae-103">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8b4ae-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b4ae-104">Получает список объектов [секурескореконтролпрофиле](../resources/securescorecontrolprofiles.md) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b4ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b4ae-105">Permissions</span></span>

<span data-ttu-id="8b4ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b4ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b4ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b4ae-108">Permission type</span></span>      | <span data-ttu-id="8b4ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b4ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b4ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b4ae-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8b4ae-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="8b4ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b4ae-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8b4ae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-113">Not supported.</span></span>  |
|<span data-ttu-id="8b4ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b4ae-114">Application</span></span> | <span data-ttu-id="8b4ae-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b4ae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b4ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="8b4ae-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b4ae-117">Request headers</span></span>

| <span data-ttu-id="8b4ae-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8b4ae-118">Name</span></span>      |<span data-ttu-id="8b4ae-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8b4ae-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b4ae-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b4ae-120">Authorization</span></span>  | <span data-ttu-id="8b4ae-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-121">Bearer {code}.</span></span> <span data-ttu-id="8b4ae-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b4ae-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b4ae-123">Request body</span></span>

<span data-ttu-id="8b4ae-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b4ae-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b4ae-125">Response</span></span>

<span data-ttu-id="8b4ae-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **секурескореконтролпрофиле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b4ae-127">Пример</span><span class="sxs-lookup"><span data-stu-id="8b4ae-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b4ae-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b4ae-128">Request</span></span>

<span data-ttu-id="8b4ae-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="8b4ae-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b4ae-130">Response</span></span>

<span data-ttu-id="8b4ae-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b4ae-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "actionType": "actionType.value",
            "actionUrl": "actionUrl.value",
            "controlCategory": "controlCategory.value",
            "title": "title.value",
            "deprecated": true,
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": 1020.13,
            "rank": 100,
            "remediation": "remediation.value",
            "remediationImpact": "remediationImpact.value",
            "service": "service.value",
            "threats": [
                "threats.value"
            ],
            "tier": "tier.value",
            "userImpact": "userImpact.value",
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "controlStateUpdates": [
                {
                    "assignedTo": "assignedTo.value",
                    "comment": "comment.value",
                    "state": "state.value",
                    "updatedBy": "updatedBy.value",
                    "updatedDateTime": "updatedDateTime.value"
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8b4ae-132">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="8b4ae-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8b4ae-133">Языках</span><span class="sxs-lookup"><span data-stu-id="8b4ae-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b4ae-134">Язык</span><span class="sxs-lookup"><span data-stu-id="8b4ae-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
