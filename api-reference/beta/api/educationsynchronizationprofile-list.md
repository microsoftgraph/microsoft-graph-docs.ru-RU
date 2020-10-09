---
title: Список Едукатионсинчронизатионпрофилес
description: Получение коллекции профилей синхронизации учебных данных в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 594627b402c386b86958c76cd4f2d67a93e6edec
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403299"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="14d4e-103">Список Едукатионсинчронизатионпрофилес</span><span class="sxs-lookup"><span data-stu-id="14d4e-103">List educationSynchronizationProfiles</span></span>

<span data-ttu-id="14d4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14d4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14d4e-105">Получение коллекции [профилей синхронизации](../resources/educationsynchronizationprofile.md) учебных данных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="14d4e-105">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="14d4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14d4e-106">Permissions</span></span>
<span data-ttu-id="14d4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14d4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14d4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14d4e-109">Permission type</span></span> | <span data-ttu-id="14d4e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14d4e-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="14d4e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14d4e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="14d4e-112">Едуадминистратион. Read, Едуадминистратион. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14d4e-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="14d4e-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14d4e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="14d4e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14d4e-114">Not supported.</span></span>|
|<span data-ttu-id="14d4e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14d4e-115">Application</span></span>|<span data-ttu-id="14d4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14d4e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14d4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14d4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14d4e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="14d4e-118">Optional query parameters</span></span>
<span data-ttu-id="14d4e-119">Этот метод поддерживает следующие [Параметры запроса OData](/graph/query-parameters) для настройки отклика: $filter, $orderby, $top, $skip и $Count.</span><span class="sxs-lookup"><span data-stu-id="14d4e-119">This method supports the following [OData Query Parameters](/graph/query-parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14d4e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14d4e-120">Request headers</span></span>
| <span data-ttu-id="14d4e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="14d4e-121">Name</span></span>       | <span data-ttu-id="14d4e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="14d4e-122">Type</span></span> | <span data-ttu-id="14d4e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="14d4e-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14d4e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14d4e-124">Authorization</span></span>  | <span data-ttu-id="14d4e-125">string</span><span class="sxs-lookup"><span data-stu-id="14d4e-125">string</span></span>  | <span data-ttu-id="14d4e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14d4e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14d4e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14d4e-128">Request body</span></span>
<span data-ttu-id="14d4e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14d4e-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="14d4e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="14d4e-130">Response</span></span>
<span data-ttu-id="14d4e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14d4e-131">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14d4e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="14d4e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14d4e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="14d4e-133">Request</span></span>
<span data-ttu-id="14d4e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14d4e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="14d4e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="14d4e-135">Response</span></span>
<span data-ttu-id="14d4e-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14d4e-136">The following is an example of the response.</span></span> 

><span data-ttu-id="14d4e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14d4e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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