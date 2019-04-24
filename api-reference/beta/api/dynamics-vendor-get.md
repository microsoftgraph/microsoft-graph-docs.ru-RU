---
title: Получение поставщиков
description: Возвращает объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ffd7476ca8412af4858df17d9c415431eaa301dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458490"
---
# <a name="get-vendors"></a><span data-ttu-id="3b773-103">Получение поставщиков</span><span class="sxs-lookup"><span data-stu-id="3b773-103">Get vendors</span></span>
<span data-ttu-id="3b773-104">Получение свойств и связей объекта Vendor для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="3b773-104">Retrieve the properties and relationships of a vendor object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b773-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b773-105">Permissions</span></span>
<span data-ttu-id="3b773-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b773-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b773-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b773-108">Permission type</span></span> |<span data-ttu-id="3b773-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b773-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3b773-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b773-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3b773-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b773-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3b773-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b773-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3b773-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b773-113">Not supported.</span></span>|
|<span data-ttu-id="3b773-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b773-114">Application</span></span>|<span data-ttu-id="3b773-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b773-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b773-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b773-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/vendors('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b773-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b773-117">Optional query parameters</span></span>
<span data-ttu-id="3b773-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3b773-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b773-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b773-119">Request headers</span></span>
|<span data-ttu-id="3b773-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b773-120">Header</span></span>|<span data-ttu-id="3b773-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3b773-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="3b773-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b773-122">Authorization</span></span>  |<span data-ttu-id="3b773-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b773-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b773-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b773-125">Request body</span></span>
<span data-ttu-id="3b773-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b773-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b773-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b773-127">Response</span></span>
<span data-ttu-id="3b773-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **вендоров** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b773-128">If successful, this method returns a `200 OK` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b773-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3b773-129">Example</span></span>

<span data-ttu-id="3b773-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="3b773-130">**Request**</span></span>

<span data-ttu-id="3b773-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b773-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/vendors('{id}')
```

<span data-ttu-id="3b773-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="3b773-132">**Response**</span></span>

<span data-ttu-id="3b773-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b773-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="3b773-134">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3b773-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3b773-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b773-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyId": "id-value",
  "currencyCode": "USD",
  "irs1099Code": "",
  "paymentTermsId": "id-value",
  "paymentMethodId": "id-value",
  "taxLiable": true,
  "blocked": " ",
  "balance": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:29.667Z"
}
```


