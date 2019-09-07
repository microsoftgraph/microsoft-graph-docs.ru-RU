---
title: Получение сотрудников
description: Возвращает объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f82730cf810caa0e8aebd2bbc9dfd323871d2a4a
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791640"
---
# <a name="get-employees"></a><span data-ttu-id="00441-103">Получение сотрудников</span><span class="sxs-lookup"><span data-stu-id="00441-103">Get employees</span></span>
<span data-ttu-id="00441-104">Получение свойств и связей объекта Employee для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="00441-104">Retrieve the properties and relationships of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="00441-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00441-105">Permissions</span></span>
<span data-ttu-id="00441-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00441-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00441-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00441-108">Permission type</span></span> |<span data-ttu-id="00441-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00441-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="00441-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00441-110">Delegated (work or school account)</span></span>|<span data-ttu-id="00441-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00441-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="00441-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00441-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="00441-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00441-113">Not supported.</span></span>|
|<span data-ttu-id="00441-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00441-114">Application</span></span>|<span data-ttu-id="00441-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00441-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00441-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00441-116">HTTP request</span></span>
```
GET /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00441-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="00441-117">Optional query parameters</span></span>
<span data-ttu-id="00441-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="00441-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00441-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00441-119">Request headers</span></span>
|<span data-ttu-id="00441-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00441-120">Header</span></span>       |<span data-ttu-id="00441-121">Значение</span><span class="sxs-lookup"><span data-stu-id="00441-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="00441-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00441-122">Authorization</span></span>|<span data-ttu-id="00441-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00441-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00441-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00441-125">Request body</span></span>
<span data-ttu-id="00441-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00441-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00441-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="00441-127">Response</span></span>
<span data-ttu-id="00441-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **Employees** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00441-128">If successful, this method returns a `200 OK` response code and an **employees** object in the response body.</span></span>

<span data-ttu-id="00441-129">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="00441-129">**Request**</span></span>

<span data-ttu-id="00441-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00441-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
```

<span data-ttu-id="00441-131">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="00441-131">**Response**</span></span>

<span data-ttu-id="00441-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00441-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="00441-133">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="00441-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="00441-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00441-134">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "AH",
  "displayName": "Annette Hill",
  "givenName": "Annette",
  "middleName": "",
  "surname": "Hill",
  "jobTitle": "Secretary",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "email": "",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "terminationDate": "0001-01-01",
  "status": "Active",
  "birthDate": "1973-12-12",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies/{id}/employees/{id}/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"  
}
```


