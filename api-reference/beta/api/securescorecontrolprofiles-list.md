---
title: Перечисление объектов secureScoreControlProfiles
description: Получение свойств и связей объекта Секурескореконтролпрофилес.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: b66f17fb7752ab129f2e1f78e25df590b5a9e79e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812575"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="8f67b-103">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8f67b-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="8f67b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f67b-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f67b-105">Получает список объектов [секурескореконтролпрофиле](../resources/securescorecontrolprofiles.md) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f67b-105">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f67b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f67b-106">Permissions</span></span>

<span data-ttu-id="8f67b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f67b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f67b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f67b-109">Permission type</span></span>      | <span data-ttu-id="8f67b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f67b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f67b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f67b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="8f67b-112">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="8f67b-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="8f67b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f67b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8f67b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f67b-114">Not supported.</span></span>  |
|<span data-ttu-id="8f67b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8f67b-115">Application</span></span> | <span data-ttu-id="8f67b-116">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="8f67b-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f67b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f67b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="8f67b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f67b-118">Request headers</span></span>

| <span data-ttu-id="8f67b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f67b-119">Name</span></span>      |<span data-ttu-id="8f67b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f67b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f67b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f67b-121">Authorization</span></span>  | <span data-ttu-id="8f67b-122">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="8f67b-122">Bearer {code}.</span></span> <span data-ttu-id="8f67b-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8f67b-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f67b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f67b-124">Request body</span></span>

<span data-ttu-id="8f67b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f67b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f67b-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f67b-126">Response</span></span>

<span data-ttu-id="8f67b-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **секурескореконтролпрофиле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f67b-127">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f67b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8f67b-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f67b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f67b-129">Request</span></span>

<span data-ttu-id="8f67b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f67b-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f67b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f67b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```
# <a name="c"></a>[<span data-ttu-id="8f67b-132">C#</span><span class="sxs-lookup"><span data-stu-id="8f67b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f67b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f67b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f67b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f67b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f67b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f67b-135">Response</span></span>

<span data-ttu-id="8f67b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f67b-136">The following is an example of the response.</span></span>
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
