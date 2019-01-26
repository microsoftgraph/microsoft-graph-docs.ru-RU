---
title: Перечисление объектов secureScores
description: Извлечение свойств и связи объекта secureScores.
localization_priority: Normal
ms.openlocfilehash: 034a333dec6b96919ffd01a49ed05cb16ca19a48
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573405"
---
# <a name="list-securescores"></a><span data-ttu-id="6f137-103">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="6f137-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f137-104">Извлечение свойств и связи объекта [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="6f137-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f137-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f137-105">Permissions</span></span>

<span data-ttu-id="6f137-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f137-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f137-108">Permission type</span></span>      | <span data-ttu-id="6f137-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f137-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f137-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f137-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6f137-111">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="6f137-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="6f137-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f137-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6f137-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f137-113">Not supported.</span></span>  |
|<span data-ttu-id="6f137-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f137-114">Application</span></span> | <span data-ttu-id="6f137-115">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="6f137-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f137-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f137-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="6f137-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f137-117">Request headers</span></span>

| <span data-ttu-id="6f137-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6f137-118">Name</span></span>      |<span data-ttu-id="6f137-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6f137-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6f137-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f137-120">Authorization</span></span>  | <span data-ttu-id="6f137-p102">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f137-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f137-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f137-123">Request body</span></span>

<span data-ttu-id="6f137-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f137-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f137-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f137-125">Response</span></span>

<span data-ttu-id="6f137-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **secureScores** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6f137-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f137-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6f137-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f137-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f137-128">Request</span></span>

<span data-ttu-id="6f137-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f137-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="6f137-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f137-130">Response</span></span>

<span data-ttu-id="6f137-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f137-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 12,
            "createdDate": "createdDateTime.value",
            "currentScore": 12.4566633444,
            "enabledServices": ["Skype"],
            "licensedUserCount": 12,
            "maxScore": 45.2324443,
            "id": "id.value",            
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                },
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                },
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                }
            ],
            "controlScores": [
                {
                    "@odata.type":"microsoft.graph.controlScores",
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
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
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
