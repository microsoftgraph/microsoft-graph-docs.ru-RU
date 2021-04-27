---
title: Создание сотрудников
description: Создает объект сотрудника в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3c3301019d958fcd1c1309c405726af24b19acfc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045952"
---
# <a name="create-employees"></a><span data-ttu-id="06c4d-103">Создание сотрудников</span><span class="sxs-lookup"><span data-stu-id="06c4d-103">Create employees</span></span>

<span data-ttu-id="06c4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06c4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06c4d-105">Создайте объект сотрудника в Центре бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="06c4d-105">Create an employee object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="06c4d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06c4d-106">Permissions</span></span>
<span data-ttu-id="06c4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06c4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06c4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06c4d-109">Permission type</span></span> |<span data-ttu-id="06c4d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06c4d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="06c4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06c4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06c4d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c4d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="06c4d-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06c4d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="06c4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c4d-114">Not supported.</span></span>|
|<span data-ttu-id="06c4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06c4d-115">Application</span></span>|<span data-ttu-id="06c4d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c4d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06c4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06c4d-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/employees
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06c4d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06c4d-118">Optional query parameters</span></span>
<span data-ttu-id="06c4d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="06c4d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06c4d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06c4d-120">Request headers</span></span>
|<span data-ttu-id="06c4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06c4d-121">Header</span></span>        |<span data-ttu-id="06c4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06c4d-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="06c4d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06c4d-123">Authorization</span></span> |<span data-ttu-id="06c4d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06c4d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="06c4d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06c4d-126">Content-Type</span></span>  |<span data-ttu-id="06c4d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="06c4d-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="06c4d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06c4d-128">Request body</span></span>
<span data-ttu-id="06c4d-129">В теле запроса поставляют представление JSON объекта **сотрудников.**</span><span class="sxs-lookup"><span data-stu-id="06c4d-129">In the request body, supply a JSON representation of an **employees** object.</span></span>

## <a name="response"></a><span data-ttu-id="06c4d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="06c4d-130">Response</span></span>
<span data-ttu-id="06c4d-131">В случае успешной работы этот метод возвращает код ответа и ```201 Created``` объект **сотрудников** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="06c4d-131">If successful, this method returns ```201 Created``` response code and an **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06c4d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="06c4d-132">Example</span></span>

<span data-ttu-id="06c4d-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="06c4d-133">**Request**</span></span>

<span data-ttu-id="06c4d-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06c4d-134">Here is an example of a request.</span></span>

```http
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

<span data-ttu-id="06c4d-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="06c4d-135">**Response**</span></span>

<span data-ttu-id="06c4d-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06c4d-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="06c4d-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06c4d-137">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
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



