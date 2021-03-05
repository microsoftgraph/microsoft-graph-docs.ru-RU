---
title: Обновление сотрудников
description: Обновляет объект сотрудника в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8c10fa7fb45642bfe988a81f22ee2a27023e777d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473079"
---
# <a name="update-employees"></a><span data-ttu-id="cdf23-103">Обновление сотрудников</span><span class="sxs-lookup"><span data-stu-id="cdf23-103">Update employees</span></span>

<span data-ttu-id="cdf23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdf23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdf23-105">Обновление свойств объекта сотрудника для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="cdf23-105">Update the properties of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdf23-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdf23-106">Permissions</span></span>
<span data-ttu-id="cdf23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdf23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdf23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdf23-109">Permission type</span></span> |<span data-ttu-id="cdf23-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdf23-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="cdf23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdf23-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdf23-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdf23-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="cdf23-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdf23-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cdf23-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdf23-114">Not supported.</span></span>|
|<span data-ttu-id="cdf23-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdf23-115">Application</span></span>|<span data-ttu-id="cdf23-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdf23-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdf23-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdf23-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdf23-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cdf23-118">Optional query parameters</span></span>
<span data-ttu-id="cdf23-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cdf23-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdf23-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdf23-120">Request headers</span></span>
|<span data-ttu-id="cdf23-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdf23-121">Header</span></span>         |<span data-ttu-id="cdf23-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cdf23-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="cdf23-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdf23-123">Authorization</span></span>  |<span data-ttu-id="cdf23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdf23-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="cdf23-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdf23-126">Content-Type</span></span>   |<span data-ttu-id="cdf23-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="cdf23-127">application/json.</span></span>         |
|<span data-ttu-id="cdf23-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="cdf23-128">If-Match</span></span>       |<span data-ttu-id="cdf23-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cdf23-129">Required.</span></span> <span data-ttu-id="cdf23-130">Если этот заглавный запрос включен и предоставленный eTag не соответствует  текущему тегу сотрудников, сотрудники не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="cdf23-130">When this request header is included and the eTag provided does not match the current tag on the **employees**, the **employees** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdf23-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdf23-131">Request body</span></span>
<span data-ttu-id="cdf23-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cdf23-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="cdf23-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdf23-135">Response</span></span>
<span data-ttu-id="cdf23-136">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` **сотрудников** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cdf23-136">If successful, this method returns a `200 OK` response code and an updated **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdf23-137">Пример</span><span class="sxs-lookup"><span data-stu-id="cdf23-137">Example</span></span>

<span data-ttu-id="cdf23-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="cdf23-138">**Request**</span></span>

<span data-ttu-id="cdf23-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdf23-139">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
Content-type: application/json

{
  "givenName": "Anthony",
  "phoneNumber": "0678-8712-3455"
}
```

<span data-ttu-id="cdf23-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="cdf23-140">**Response**</span></span>

<span data-ttu-id="cdf23-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cdf23-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="cdf23-142">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cdf23-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cdf23-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdf23-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "displayName": "Anthony Hill",
  "givenName": "Anthony",
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
  "phoneNumber": "0678-8712-3455",
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
  


