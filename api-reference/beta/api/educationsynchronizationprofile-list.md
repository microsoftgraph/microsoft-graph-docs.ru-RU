---
title: Список Едукатионсинчронизатионпрофилес
description: Получение коллекции профилей синхронизации учебных данных в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1907b0ef08473a79d66e79fcb4751b281e9a18ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457467"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="78880-103">Список Едукатионсинчронизатионпрофилес</span><span class="sxs-lookup"><span data-stu-id="78880-103">List educationSynchronizationProfiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78880-104">Получение коллекции [профилей синхронизации](../resources/educationsynchronizationprofile.md) учебных данных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="78880-104">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="78880-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78880-105">Permissions</span></span>
<span data-ttu-id="78880-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78880-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78880-108">Permission type</span></span> | <span data-ttu-id="78880-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78880-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="78880-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78880-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78880-111">Едуадминистратион. Read, Едуадминистратион. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78880-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="78880-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78880-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="78880-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78880-113">Not supported.</span></span>|
|<span data-ttu-id="78880-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78880-114">Application</span></span>|<span data-ttu-id="78880-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78880-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78880-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78880-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78880-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78880-117">Optional query parameters</span></span>
<span data-ttu-id="78880-118">Этот метод поддерживает следующие [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика: $filter, $orderby, $top, $skip и $Count.</span><span class="sxs-lookup"><span data-stu-id="78880-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78880-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78880-119">Request headers</span></span>
| <span data-ttu-id="78880-120">Имя</span><span class="sxs-lookup"><span data-stu-id="78880-120">Name</span></span>       | <span data-ttu-id="78880-121">Тип</span><span class="sxs-lookup"><span data-stu-id="78880-121">Type</span></span> | <span data-ttu-id="78880-122">Описание</span><span class="sxs-lookup"><span data-stu-id="78880-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="78880-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78880-123">Authorization</span></span>  | <span data-ttu-id="78880-124">string</span><span class="sxs-lookup"><span data-stu-id="78880-124">string</span></span>  | <span data-ttu-id="78880-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78880-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="78880-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78880-127">Request body</span></span>
<span data-ttu-id="78880-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78880-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="78880-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="78880-129">Response</span></span>
<span data-ttu-id="78880-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="78880-130">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78880-131">Пример</span><span class="sxs-lookup"><span data-stu-id="78880-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78880-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="78880-132">Request</span></span>
<span data-ttu-id="78880-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78880-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="78880-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="78880-134">Response</span></span>
<span data-ttu-id="78880-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="78880-135">The following is an example of the response.</span></span> 

><span data-ttu-id="78880-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78880-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3296

{
    "value": [
    {
        "displayName": "Test Profile",
        "state": "provisioned",
        "id": "15e9b9fa-de85-492e-aa44-550c40de626e",
        "dataProvider": {
            "@odata.type": "microsoft.graph.educationCsvDataProvider",
            "customizations": {
                "school": {
                    "optionalPropertiesToSync": [
                        "School NCES_ID",
                        "State ID",
                        "GradeLow",
                        "GradeHigh",
                        "Principal Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "section": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "student": {
                    "optionalPropertiesToSync": [
                        "State ID",
                        "Email",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacher": {
                    "optionalPropertiesToSync": [
                        "Teacher Number",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "studentEnrollment": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacherRoster": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                }
            }
        },
        "identitySynchronizationConfiguration": {
            "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
            "userDomains": [
                {
                    "appliesTo": "student",
                    "name": "testschool.edu"
                },
                {
                    "appliesTo": "teacher",
                    "name": "testschool.edu"
                }
            ]
        },
        "licensesToAssign": [
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",                
                "appliesTo": "teacher",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            },
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
                "appliesTo": "student",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            }
        ]
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
