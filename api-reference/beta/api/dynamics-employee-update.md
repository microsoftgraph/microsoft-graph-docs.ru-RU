---
title: Обновление сотрудников
description: Обновляет объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ac17678b5cc75d8416918b6f39583d27f9d5dea7
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791661"
---
# <a name="update-employees"></a><span data-ttu-id="be4b8-103">Обновление сотрудников</span><span class="sxs-lookup"><span data-stu-id="be4b8-103">Update employees</span></span>
<span data-ttu-id="be4b8-104">Обновление свойств объекта Employee для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="be4b8-104">Update the properties of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="be4b8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be4b8-105">Permissions</span></span>
<span data-ttu-id="be4b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be4b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be4b8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be4b8-108">Permission type</span></span> |<span data-ttu-id="be4b8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be4b8-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="be4b8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be4b8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="be4b8-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4b8-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="be4b8-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be4b8-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="be4b8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be4b8-113">Not supported.</span></span>|
|<span data-ttu-id="be4b8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be4b8-114">Application</span></span>|<span data-ttu-id="be4b8-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4b8-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be4b8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be4b8-116">HTTP request</span></span>

```
PATCH /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be4b8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be4b8-117">Optional query parameters</span></span>
<span data-ttu-id="be4b8-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be4b8-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be4b8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be4b8-119">Request headers</span></span>
|<span data-ttu-id="be4b8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be4b8-120">Header</span></span>         |<span data-ttu-id="be4b8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="be4b8-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="be4b8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be4b8-122">Authorization</span></span>  |<span data-ttu-id="be4b8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be4b8-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="be4b8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be4b8-125">Content-Type</span></span>   |<span data-ttu-id="be4b8-126">application/json.</span><span class="sxs-lookup"><span data-stu-id="be4b8-126">application/json.</span></span>         |
|<span data-ttu-id="be4b8-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="be4b8-127">If-Match</span></span>       |<span data-ttu-id="be4b8-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="be4b8-128">Required.</span></span> <span data-ttu-id="be4b8-129">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу **сотрудников**, **сотрудники** не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="be4b8-129">When this request header is included and the eTag provided does not match the current tag on the **employees**, the **employees** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be4b8-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be4b8-130">Request body</span></span>
<span data-ttu-id="be4b8-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="be4b8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="be4b8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="be4b8-134">Response</span></span>
<span data-ttu-id="be4b8-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект **Employees** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be4b8-135">If successful, this method returns a `200 OK` response code and an updated **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be4b8-136">Пример</span><span class="sxs-lookup"><span data-stu-id="be4b8-136">Example</span></span>

<span data-ttu-id="be4b8-137">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="be4b8-137">**Request**</span></span>

<span data-ttu-id="be4b8-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be4b8-138">Here is an example of the request.</span></span>

```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
Content-type: application/json

{
  "givenName": "Anthony",
  "phoneNumber": "0678-8712-3455"
}
```

<span data-ttu-id="be4b8-139">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="be4b8-139">**Response**</span></span>

<span data-ttu-id="be4b8-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be4b8-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="be4b8-141">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="be4b8-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be4b8-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be4b8-142">All the properties will be returned from an actual call.</span></span>

```json
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
  
