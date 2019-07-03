---
title: Перечисление объектов secureScoreControlProfiles
description: Получение свойств и связей объекта Секурескореконтролпрофилес.
localization_priority: Normal
ms.openlocfilehash: b4bc25e8ed9820824f26a3380ef53e20ae08af45
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453798"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="ba888-103">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="ba888-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba888-104">Получает список объектов [секурескореконтролпрофиле](../resources/securescorecontrolprofiles.md) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba888-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba888-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba888-105">Permissions</span></span>

<span data-ttu-id="ba888-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba888-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba888-108">Permission type</span></span>      | <span data-ttu-id="ba888-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba888-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba888-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba888-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ba888-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="ba888-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="ba888-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba888-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ba888-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba888-113">Not supported.</span></span>  |
|<span data-ttu-id="ba888-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba888-114">Application</span></span> | <span data-ttu-id="ba888-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="ba888-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba888-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba888-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ba888-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba888-117">Request headers</span></span>

| <span data-ttu-id="ba888-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ba888-118">Name</span></span>      |<span data-ttu-id="ba888-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ba888-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba888-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba888-120">Authorization</span></span>  | <span data-ttu-id="ba888-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="ba888-121">Bearer {code}.</span></span> <span data-ttu-id="ba888-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ba888-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba888-123">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="ba888-123">Request body</span></span>

<span data-ttu-id="ba888-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba888-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba888-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba888-125">Response</span></span>

<span data-ttu-id="ba888-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **секурескореконтролпрофиле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba888-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba888-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ba888-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba888-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba888-128">Request</span></span>

<span data-ttu-id="ba888-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba888-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba888-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba888-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba888-131">C#</span><span class="sxs-lookup"><span data-stu-id="ba888-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba888-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba888-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba888-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ba888-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba888-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba888-134">Response</span></span>

<span data-ttu-id="ba888-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ba888-135">The following is an example of the response.</span></span>
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
