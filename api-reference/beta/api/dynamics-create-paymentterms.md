---
title: Создание Пайменттермс
description: Создает объект условий оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 40f39f94f0249e2fa9947d8b3f828fc344a1ed39
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791920"
---
# <a name="create-paymentterms"></a><span data-ttu-id="6aa3f-103">Создание Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6aa3f-103">Create paymentTerms</span></span>
<span data-ttu-id="6aa3f-104">Создайте объект условий оплаты в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-104">Create a payment terms object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6aa3f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa3f-105">Permissions</span></span>
<span data-ttu-id="6aa3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aa3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aa3f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa3f-108">Permission type</span></span> |<span data-ttu-id="6aa3f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa3f-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6aa3f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa3f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6aa3f-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aa3f-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6aa3f-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa3f-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6aa3f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-113">Not supported.</span></span>|
|<span data-ttu-id="6aa3f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6aa3f-114">Application</span></span>|<span data-ttu-id="6aa3f-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aa3f-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aa3f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aa3f-116">HTTP request</span></span>
```
POST /financials/companies/{id}/paymentTerms
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6aa3f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6aa3f-117">Optional query parameters</span></span>
<span data-ttu-id="6aa3f-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6aa3f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6aa3f-119">Request headers</span></span>
|<span data-ttu-id="6aa3f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6aa3f-120">Header</span></span>|<span data-ttu-id="6aa3f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6aa3f-121">Value</span></span>|
|---------------|-----------------------------|
|<span data-ttu-id="6aa3f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6aa3f-122">Authorization</span></span>  |<span data-ttu-id="6aa3f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="6aa3f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6aa3f-125">Content-Type</span></span>   |<span data-ttu-id="6aa3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6aa3f-126">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="6aa3f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6aa3f-127">Request body</span></span>
<span data-ttu-id="6aa3f-128">В тексте запроса добавьте представление объекта **пайменттермс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-128">In the request body, supply a JSON representation of a **paymentTerms** object.</span></span>

## <a name="response"></a><span data-ttu-id="6aa3f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aa3f-129">Response</span></span>
<span data-ttu-id="6aa3f-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **пайменттермс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-130">If successful, this method returns ```201 Created``` response code and a **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aa3f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6aa3f-131">Example</span></span>

<span data-ttu-id="6aa3f-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="6aa3f-132">**Request**</span></span>

<span data-ttu-id="6aa3f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentTerms
Content-type: application/json

{
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false
}
```

<span data-ttu-id="6aa3f-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="6aa3f-134">**Response**</span></span>

<span data-ttu-id="6aa3f-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="6aa3f-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6aa3f-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6aa3f-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false,
  "lastModifiedDateTime": "2017-03-03T02:14:32Z"
}

```
