---
title: Создание Пайменттермс
description: Создает объект условий оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 84a756dc92819a2ab40b6bc24600af9c66f2004c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956599"
---
# <a name="create-paymentterms"></a><span data-ttu-id="734b3-103">Создание Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="734b3-103">Create paymentTerms</span></span>
<span data-ttu-id="734b3-104">Создайте объект условий оплаты в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="734b3-104">Create a payment terms object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="734b3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="734b3-105">Permissions</span></span>
<span data-ttu-id="734b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="734b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="734b3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="734b3-108">Permission type</span></span> |<span data-ttu-id="734b3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="734b3-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="734b3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="734b3-110">Delegated (work or school account)</span></span>|<span data-ttu-id="734b3-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="734b3-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="734b3-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="734b3-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="734b3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="734b3-113">Not supported.</span></span>|
|<span data-ttu-id="734b3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="734b3-114">Application</span></span>|<span data-ttu-id="734b3-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="734b3-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="734b3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="734b3-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/paymentTerms
```

## <a name="optional-query-parameters"></a><span data-ttu-id="734b3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="734b3-117">Optional query parameters</span></span>
<span data-ttu-id="734b3-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="734b3-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="734b3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="734b3-119">Request headers</span></span>
|<span data-ttu-id="734b3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="734b3-120">Header</span></span>|<span data-ttu-id="734b3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="734b3-121">Value</span></span>|
|---------------|-----------------------------|
|<span data-ttu-id="734b3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="734b3-122">Authorization</span></span>  |<span data-ttu-id="734b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="734b3-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="734b3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="734b3-125">Content-Type</span></span>   |<span data-ttu-id="734b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="734b3-126">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="734b3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="734b3-127">Request body</span></span>
<span data-ttu-id="734b3-128">В тексте запроса добавьте представление объекта **пайменттермс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="734b3-128">In the request body, supply a JSON representation of a **paymentTerms** object.</span></span>

## <a name="response"></a><span data-ttu-id="734b3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="734b3-129">Response</span></span>
<span data-ttu-id="734b3-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **пайменттермс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="734b3-130">If successful, this method returns ```201 Created``` response code and a **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="734b3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="734b3-131">Example</span></span>

<span data-ttu-id="734b3-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="734b3-132">**Request**</span></span>

<span data-ttu-id="734b3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="734b3-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/paymentTerms
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

<span data-ttu-id="734b3-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="734b3-134">**Response**</span></span>

<span data-ttu-id="734b3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="734b3-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="734b3-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="734b3-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="734b3-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="734b3-137">All the properties will be returned from an actual call.</span></span>

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
