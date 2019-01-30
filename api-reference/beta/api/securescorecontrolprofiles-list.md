---
title: Перечисление объектов secureScoreControlProfiles
description: Извлечение свойств и связи объекта secureScoreControlProfiles.
localization_priority: Normal
ms.openlocfilehash: 6627111633f54eb7bc2584af826b69fd5bd6cf49
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644030"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="0a557-103">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="0a557-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a557-104">Извлечение свойств и связи объекта [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) .</span><span class="sxs-lookup"><span data-stu-id="0a557-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a557-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a557-105">Permissions</span></span>

<span data-ttu-id="0a557-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a557-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a557-108">Permission type</span></span>      | <span data-ttu-id="0a557-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a557-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a557-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a557-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0a557-111">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="0a557-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="0a557-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a557-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0a557-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a557-113">Not supported.</span></span>  |
|<span data-ttu-id="0a557-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a557-114">Application</span></span> | <span data-ttu-id="0a557-115">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="0a557-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a557-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a557-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0a557-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a557-117">Request headers</span></span>

| <span data-ttu-id="0a557-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0a557-118">Name</span></span>      |<span data-ttu-id="0a557-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0a557-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a557-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a557-120">Authorization</span></span>  | <span data-ttu-id="0a557-p102">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a557-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a557-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a557-123">Request body</span></span>

<span data-ttu-id="0a557-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a557-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a557-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a557-125">Response</span></span>

<span data-ttu-id="0a557-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **secureScoreControlProfiles** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a557-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a557-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0a557-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a557-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a557-128">Request</span></span>

<span data-ttu-id="0a557-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a557-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="0a557-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a557-130">Response</span></span>

<span data-ttu-id="0a557-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a557-131">The following is an example of the response.</span></span>
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
