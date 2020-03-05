---
title: Создание сотрудников
description: Создает объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e58f0f3c44d9ed7e78ecdd8176d4710e89542f7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431587"
---
# <a name="create-employees"></a><span data-ttu-id="c399a-103">Создание сотрудников</span><span class="sxs-lookup"><span data-stu-id="c399a-103">Create employees</span></span>

<span data-ttu-id="c399a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c399a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c399a-105">Создайте объект Employee в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="c399a-105">Create an employee object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="c399a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c399a-106">Permissions</span></span>
<span data-ttu-id="c399a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c399a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c399a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c399a-109">Permission type</span></span> |<span data-ttu-id="c399a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c399a-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c399a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c399a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c399a-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c399a-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c399a-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c399a-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c399a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c399a-114">Not supported.</span></span>|
|<span data-ttu-id="c399a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c399a-115">Application</span></span>|<span data-ttu-id="c399a-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c399a-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c399a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c399a-117">HTTP request</span></span>
```
POST /financials/companies/{id}/employees
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c399a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c399a-118">Optional query parameters</span></span>
<span data-ttu-id="c399a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c399a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c399a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c399a-120">Request headers</span></span>
|<span data-ttu-id="c399a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c399a-121">Header</span></span>        |<span data-ttu-id="c399a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c399a-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="c399a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c399a-123">Authorization</span></span> |<span data-ttu-id="c399a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c399a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c399a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c399a-126">Content-Type</span></span>  |<span data-ttu-id="c399a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c399a-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="c399a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c399a-128">Request body</span></span>
<span data-ttu-id="c399a-129">В тексте запроса добавьте представление объекта **Employees** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c399a-129">In the request body, supply a JSON representation of an **employees** object.</span></span>

## <a name="response"></a><span data-ttu-id="c399a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c399a-130">Response</span></span>
<span data-ttu-id="c399a-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **Employees** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c399a-131">If successful, this method returns ```201 Created``` response code and an **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c399a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c399a-132">Example</span></span>

<span data-ttu-id="c399a-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="c399a-133">**Request**</span></span>

<span data-ttu-id="c399a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c399a-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/employees
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "givenName": "Annette",
  "surname": "Hill",
  "jobTitle": "Production Assistant",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "birthDate": "1973-12-12"  
}

```

<span data-ttu-id="c399a-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="c399a-135">**Response**</span></span>

<span data-ttu-id="c399a-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c399a-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="c399a-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c399a-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c399a-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c399a-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

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

