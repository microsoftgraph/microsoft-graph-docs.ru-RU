---
title: Получение educationSynchronizationErrors
description: 'Получите ошибки, возникающие во время проверки и/или во время синхронизации профиля синхронизации данных конкретного school в клиентов. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 48afa5ce7efc267eedc16449324980e527409dc9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425129"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="7186b-103">Получение educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="7186b-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="7186b-104">Получите ошибки, возникающие во время проверки и/или во время синхронизации данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиента.</span><span class="sxs-lookup"><span data-stu-id="7186b-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7186b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7186b-105">Permissions</span></span>
<span data-ttu-id="7186b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7186b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7186b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7186b-108">Permission type</span></span> | <span data-ttu-id="7186b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7186b-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="7186b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7186b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7186b-111">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7186b-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="7186b-112">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="7186b-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7186b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7186b-113">Not supported.</span></span>|
|<span data-ttu-id="7186b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7186b-114">Application</span></span>| <span data-ttu-id="7186b-115">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7186b-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7186b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7186b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7186b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7186b-117">Optional query parameters</span></span>
<span data-ttu-id="7186b-118">Этот метод поддерживает следующие [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа: $filter, $orderby, $top, $skip и $count.</span><span class="sxs-lookup"><span data-stu-id="7186b-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7186b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7186b-119">Request headers</span></span>
| <span data-ttu-id="7186b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7186b-120">Name</span></span>       | <span data-ttu-id="7186b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7186b-121">Type</span></span> | <span data-ttu-id="7186b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7186b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7186b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7186b-123">Authorization</span></span>  | <span data-ttu-id="7186b-124">string</span><span class="sxs-lookup"><span data-stu-id="7186b-124">string</span></span>  | <span data-ttu-id="7186b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7186b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7186b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7186b-127">Request body</span></span>
<span data-ttu-id="7186b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7186b-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7186b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7186b-129">Response</span></span>
<span data-ttu-id="7186b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [Ошибка синхронизации](../resources/educationsynchronizationerror.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7186b-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7186b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7186b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7186b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7186b-132">Request</span></span>
<span data-ttu-id="7186b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7186b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```

##### <a name="response"></a><span data-ttu-id="7186b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7186b-134">Response</span></span>
<span data-ttu-id="7186b-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7186b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="7186b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7186b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/errors",
    "@odata.count": 14,
    "value": [
        {
            "entryType": "Student",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
            "joiningValue": "richard.2wilson@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:45Z",
            "reportableIdentifier": "richard.2wilson"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "alberto2.dorsey@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "alberto2.dorsey"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "madeline2.bullock@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "madeline2.bullock"
        }
    ]
}
```
