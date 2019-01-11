---
title: Перечисление объектов secureScoreControlProfiles
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: cd13e4349119202f5f9e026973f3a90ee99f1019
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884555"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="44762-104">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="44762-104">List secureScoreControlProfiles</span></span>

 > <span data-ttu-id="44762-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44762-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44762-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44762-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44762-107">Извлечение свойств и связи объекта [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) .</span><span class="sxs-lookup"><span data-stu-id="44762-107">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44762-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44762-108">Permissions</span></span>

<span data-ttu-id="44762-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44762-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44762-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44762-111">Permission type</span></span>      | <span data-ttu-id="44762-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44762-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44762-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44762-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="44762-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="44762-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="44762-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44762-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="44762-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44762-116">Not supported.</span></span>  |
|<span data-ttu-id="44762-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44762-117">Application</span></span> | <span data-ttu-id="44762-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="44762-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44762-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44762-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="44762-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44762-120">Request headers</span></span>

| <span data-ttu-id="44762-121">Имя</span><span class="sxs-lookup"><span data-stu-id="44762-121">Name</span></span>      |<span data-ttu-id="44762-122">Описание</span><span class="sxs-lookup"><span data-stu-id="44762-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="44762-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44762-123">Authorization</span></span>  | <span data-ttu-id="44762-p104">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44762-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44762-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44762-126">Request body</span></span>

<span data-ttu-id="44762-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44762-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44762-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="44762-128">Response</span></span>

<span data-ttu-id="44762-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **secureScoreControlProfiles** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="44762-129">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44762-130">Пример</span><span class="sxs-lookup"><span data-stu-id="44762-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="44762-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="44762-131">Request</span></span>

<span data-ttu-id="44762-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44762-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="44762-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="44762-133">Response</span></span>

<span data-ttu-id="44762-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="44762-134">The following is an example of the response.</span></span>
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


<!-- {
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
