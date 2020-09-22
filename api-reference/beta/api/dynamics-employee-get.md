---
title: Получение сотрудников
description: Возвращает объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2309889f58575f2e8b50a6fe3d31c98700d5fb9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981331"
---
# <a name="get-employees"></a><span data-ttu-id="9977e-103">Получение сотрудников</span><span class="sxs-lookup"><span data-stu-id="9977e-103">Get employees</span></span>

<span data-ttu-id="9977e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9977e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9977e-105">Получение свойств и связей объекта Employee для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9977e-105">Retrieve the properties and relationships of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9977e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9977e-106">Permissions</span></span>
<span data-ttu-id="9977e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9977e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9977e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9977e-109">Permission type</span></span> |<span data-ttu-id="9977e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9977e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9977e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9977e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9977e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9977e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9977e-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9977e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9977e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9977e-114">Not supported.</span></span>|
|<span data-ttu-id="9977e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9977e-115">Application</span></span>|<span data-ttu-id="9977e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9977e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9977e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9977e-117">HTTP request</span></span>
```
GET /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9977e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9977e-118">Optional query parameters</span></span>
<span data-ttu-id="9977e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9977e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9977e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9977e-120">Request headers</span></span>
|<span data-ttu-id="9977e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9977e-121">Header</span></span>       |<span data-ttu-id="9977e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9977e-122">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="9977e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9977e-123">Authorization</span></span>|<span data-ttu-id="9977e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9977e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9977e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9977e-126">Request body</span></span>
<span data-ttu-id="9977e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9977e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9977e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9977e-128">Response</span></span>
<span data-ttu-id="9977e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **Employees** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9977e-129">If successful, this method returns a `200 OK` response code and an **employees** object in the response body.</span></span>

<span data-ttu-id="9977e-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="9977e-130">**Request**</span></span>

<span data-ttu-id="9977e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9977e-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
```

<span data-ttu-id="9977e-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="9977e-132">**Response**</span></span>

<span data-ttu-id="9977e-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9977e-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="9977e-134">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9977e-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9977e-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9977e-135">All the properties will be returned from an actual call.</span></span>

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




