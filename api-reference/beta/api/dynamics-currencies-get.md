---
title: Получение валют
description: Возвращает объект Currency в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6c8d3fdf8c6251e4764cfd61a484c287af58e53f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42430947"
---
# <a name="get-currencies"></a><span data-ttu-id="50d04-103">Получение валют</span><span class="sxs-lookup"><span data-stu-id="50d04-103">Get currencies</span></span>

<span data-ttu-id="50d04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50d04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50d04-105">Получение свойств и связей объекта Currency для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="50d04-105">Retrieve the properties and relationships of a currency object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="50d04-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50d04-106">Permissions</span></span>
<span data-ttu-id="50d04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50d04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d04-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50d04-109">Permission type</span></span> |<span data-ttu-id="50d04-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50d04-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="50d04-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50d04-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50d04-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d04-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="50d04-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50d04-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="50d04-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50d04-114">Not supported.</span></span>|
|<span data-ttu-id="50d04-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50d04-115">Application</span></span>|<span data-ttu-id="50d04-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d04-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50d04-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50d04-117">HTTP request</span></span>

```
GET /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50d04-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50d04-118">Optional query parameters</span></span>
<span data-ttu-id="50d04-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50d04-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50d04-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50d04-120">Request headers</span></span>
|<span data-ttu-id="50d04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50d04-121">Header</span></span>|<span data-ttu-id="50d04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50d04-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="50d04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50d04-123">Authorization</span></span>  |<span data-ttu-id="50d04-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50d04-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50d04-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50d04-126">Request body</span></span>
<span data-ttu-id="50d04-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50d04-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50d04-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="50d04-128">Response</span></span>
<span data-ttu-id="50d04-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **валюты** в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="50d04-129">If successful, this method returns a `200 OK` response code and a **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d04-130">Пример</span><span class="sxs-lookup"><span data-stu-id="50d04-130">Example</span></span>

<span data-ttu-id="50d04-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="50d04-131">**Request**</span></span>

<span data-ttu-id="50d04-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50d04-132">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

<span data-ttu-id="50d04-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="50d04-133">**Response**</span></span>

<span data-ttu-id="50d04-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="50d04-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="50d04-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="50d04-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="50d04-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50d04-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:05:09.003Z"
}
```
