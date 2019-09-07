---
title: Получение Пайменттермс
description: Получает объект термина платежа в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: efecba2c4a1432dfa9e16d3942f57c872f34367d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791367"
---
# <a name="get-paymentterms"></a><span data-ttu-id="a1627-103">Получение Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="a1627-103">Get paymentTerms</span></span>
<span data-ttu-id="a1627-104">Получение свойств и связей объекта условий оплаты для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a1627-104">Retrieve the properties and relationships of a payment terms object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1627-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1627-105">Permissions</span></span>
<span data-ttu-id="a1627-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1627-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1627-108">Permission type</span></span> |<span data-ttu-id="a1627-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1627-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a1627-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1627-110">Delegated (work or school account)</span></span>|<span data-ttu-id="a1627-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1627-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a1627-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1627-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a1627-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1627-113">Not supported.</span></span>|
|<span data-ttu-id="a1627-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1627-114">Application</span></span>|<span data-ttu-id="a1627-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1627-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1627-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1627-116">HTTP request</span></span>

```
GET /financials/companies/{id}/paymentTerms/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1627-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1627-117">Optional query parameters</span></span>
<span data-ttu-id="a1627-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1627-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1627-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1627-119">Request headers</span></span>
|<span data-ttu-id="a1627-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1627-120">Header</span></span>         |<span data-ttu-id="a1627-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1627-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="a1627-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1627-122">Authorization</span></span>  |<span data-ttu-id="a1627-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1627-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1627-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1627-125">Request body</span></span>
<span data-ttu-id="a1627-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1627-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1627-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1627-127">Response</span></span>
<span data-ttu-id="a1627-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **пайменттермс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1627-128">If successful, this method returns a `200 OK` response code and a **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1627-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a1627-129">Example</span></span>

<span data-ttu-id="a1627-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="a1627-130">**Request**</span></span>

<span data-ttu-id="a1627-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1627-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/paymentTerms/{id}
```

<span data-ttu-id="a1627-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="a1627-132">**Response**</span></span>

<span data-ttu-id="a1627-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1627-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="a1627-134">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a1627-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a1627-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1627-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false,
  "lastModifiedDateTime": "2017-03-15T02:20:55.203Z"
}
```
