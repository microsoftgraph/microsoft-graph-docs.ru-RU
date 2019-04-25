---
title: Перечисление объектов secureScoreControlProfiles
description: Получение свойств и связей объекта Секурескореконтролпрофилес.
localization_priority: Normal
ms.openlocfilehash: 6627111633f54eb7bc2584af826b69fd5bd6cf49
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545640"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="22059-103">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="22059-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22059-104">Получение свойств и связей объекта [секурескореконтролпрофилес](../resources/securescorecontrolprofiles.md) .</span><span class="sxs-lookup"><span data-stu-id="22059-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22059-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22059-105">Permissions</span></span>

<span data-ttu-id="22059-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22059-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22059-108">Permission type</span></span>      | <span data-ttu-id="22059-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22059-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22059-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22059-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="22059-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="22059-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="22059-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22059-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="22059-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22059-113">Not supported.</span></span>  |
|<span data-ttu-id="22059-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22059-114">Application</span></span> | <span data-ttu-id="22059-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="22059-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22059-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22059-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="22059-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22059-117">Request headers</span></span>

| <span data-ttu-id="22059-118">Имя</span><span class="sxs-lookup"><span data-stu-id="22059-118">Name</span></span>      |<span data-ttu-id="22059-119">Описание</span><span class="sxs-lookup"><span data-stu-id="22059-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22059-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22059-120">Authorization</span></span>  | <span data-ttu-id="22059-121">Bearer {Code}.</span><span class="sxs-lookup"><span data-stu-id="22059-121">Bearer {code}.</span></span> <span data-ttu-id="22059-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22059-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22059-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22059-123">Request body</span></span>

<span data-ttu-id="22059-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22059-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22059-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="22059-125">Response</span></span>

<span data-ttu-id="22059-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескореконтролпрофилес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22059-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22059-127">Пример</span><span class="sxs-lookup"><span data-stu-id="22059-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="22059-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="22059-128">Request</span></span>

<span data-ttu-id="22059-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22059-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="22059-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="22059-130">Response</span></span>

<span data-ttu-id="22059-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22059-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
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
            "deprecated": "deprecated.value",
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": "maxScore.value",
            "rank": "rank.value",
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
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
