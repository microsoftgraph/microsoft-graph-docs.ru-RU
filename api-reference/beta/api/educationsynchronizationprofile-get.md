---
title: Получение Едукатионсинчронизатионпрофиле
description: Получение профиля синхронизации данных School в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6c294ab025c148d851ee679c8b64c69608a470f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424486"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="8e5d5-103">Получение Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="8e5d5-103">Get an educationSynchronizationProfile</span></span>

<span data-ttu-id="8e5d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e5d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e5d5-105">Получение [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="8e5d5-105">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e5d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e5d5-106">Permissions</span></span>
<span data-ttu-id="8e5d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e5d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e5d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e5d5-109">Permission type</span></span> | <span data-ttu-id="8e5d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e5d5-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="8e5d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e5d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8e5d5-112">Едуадминистратион. Read, Едуадминистратион. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e5d5-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="8e5d5-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e5d5-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8e5d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e5d5-114">Not supported.</span></span>|
|<span data-ttu-id="8e5d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e5d5-115">Application</span></span>| <span data-ttu-id="8e5d5-116">Едуадминистратион. Read. ALL, Едуадминистратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8e5d5-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e5d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e5d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8e5d5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e5d5-118">Request headers</span></span>
| <span data-ttu-id="8e5d5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8e5d5-119">Name</span></span>       | <span data-ttu-id="8e5d5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8e5d5-120">Type</span></span> | <span data-ttu-id="8e5d5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8e5d5-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8e5d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e5d5-122">Authorization</span></span>  | <span data-ttu-id="8e5d5-123">string</span><span class="sxs-lookup"><span data-stu-id="8e5d5-123">string</span></span>  | <span data-ttu-id="8e5d5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e5d5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e5d5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e5d5-126">Request body</span></span>
<span data-ttu-id="8e5d5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e5d5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8e5d5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e5d5-128">Response</span></span>
<span data-ttu-id="8e5d5-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e5d5-129">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e5d5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8e5d5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e5d5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e5d5-131">Request</span></span>
<span data-ttu-id="8e5d5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e5d5-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="8e5d5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e5d5-133">Response</span></span>
<span data-ttu-id="8e5d5-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e5d5-134">The following is an example of the response.</span></span> 

><span data-ttu-id="8e5d5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e5d5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2487

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/$entity",
    "displayName": "Test Profile",
    "state": "provisioned",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacher": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Teacher Number",
                    "Status",
                    "Middle Name",
                    "Secondary Email",
                    "Title",
                    "Qualification"
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
    "licensesToAssign": 
         [
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
```
