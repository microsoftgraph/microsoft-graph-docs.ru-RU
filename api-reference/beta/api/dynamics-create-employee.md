---
title: Создание сотрудников
description: Создает объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 5432a312c4a1702b47413ee7080da0653a159fef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463651"
---
# <a name="create-employees"></a><span data-ttu-id="d1bcf-103">Создание сотрудников</span><span class="sxs-lookup"><span data-stu-id="d1bcf-103">Create employees</span></span>
<span data-ttu-id="d1bcf-104">Создайте объект Employee в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-104">Create an employee object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1bcf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1bcf-105">Permissions</span></span>
<span data-ttu-id="d1bcf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1bcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1bcf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1bcf-108">Permission type</span></span> |<span data-ttu-id="d1bcf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1bcf-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d1bcf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1bcf-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d1bcf-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bcf-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d1bcf-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1bcf-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d1bcf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-113">Not supported.</span></span>|
|<span data-ttu-id="d1bcf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1bcf-114">Application</span></span>|<span data-ttu-id="d1bcf-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bcf-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1bcf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1bcf-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/employees
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1bcf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1bcf-117">Optional query parameters</span></span>
<span data-ttu-id="d1bcf-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1bcf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1bcf-119">Request headers</span></span>
|<span data-ttu-id="d1bcf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1bcf-120">Header</span></span>        |<span data-ttu-id="d1bcf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d1bcf-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="d1bcf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1bcf-122">Authorization</span></span> |<span data-ttu-id="d1bcf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d1bcf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1bcf-125">Content-Type</span></span>  |<span data-ttu-id="d1bcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1bcf-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="d1bcf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1bcf-127">Request body</span></span>
<span data-ttu-id="d1bcf-128">В тексте запроса добавьте представление объекта Employees в формате \*\*\*\* JSON.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-128">In the request body, supply a JSON representation of an **employees** object.</span></span>

## <a name="response"></a><span data-ttu-id="d1bcf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1bcf-129">Response</span></span>
<span data-ttu-id="d1bcf-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **Employees** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-130">If successful, this method returns ```201 Created``` response code and an **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1bcf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d1bcf-131">Example</span></span>

<span data-ttu-id="d1bcf-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d1bcf-132">**Request**</span></span>

<span data-ttu-id="d1bcf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/employees
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

<span data-ttu-id="d1bcf-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d1bcf-134">**Response**</span></span>

<span data-ttu-id="d1bcf-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="d1bcf-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d1bcf-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1bcf-137">All the properties will be returned from an actual call.</span></span>

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
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/employees('{id}')/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z" 
}

```

