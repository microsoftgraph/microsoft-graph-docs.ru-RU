---
title: Создание валют
description: Создает объект Currency в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 53da84723042439505a91dee3838426db6ced820
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365873"
---
# <a name="create-currencies"></a><span data-ttu-id="335a3-103">Создание валют</span><span class="sxs-lookup"><span data-stu-id="335a3-103">Create currencies</span></span>
<span data-ttu-id="335a3-104">Создайте объект Currency в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="335a3-104">Create a currency object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="335a3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="335a3-105">Permissions</span></span>
<span data-ttu-id="335a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="335a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="335a3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="335a3-108">Permission type</span></span> |<span data-ttu-id="335a3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="335a3-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="335a3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="335a3-110">Delegated (work or school account)</span></span>|<span data-ttu-id="335a3-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="335a3-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="335a3-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="335a3-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="335a3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="335a3-113">Not supported.</span></span>|
|<span data-ttu-id="335a3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="335a3-114">Application</span></span>|<span data-ttu-id="335a3-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="335a3-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="335a3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="335a3-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/currencies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="335a3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="335a3-117">Optional query parameters</span></span>
<span data-ttu-id="335a3-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="335a3-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="335a3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="335a3-119">Request headers</span></span>
|<span data-ttu-id="335a3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="335a3-120">Header</span></span>         |<span data-ttu-id="335a3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="335a3-121">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="335a3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="335a3-122">Authorization</span></span>  |<span data-ttu-id="335a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="335a3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="335a3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="335a3-125">Content-Type</span></span>   |<span data-ttu-id="335a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="335a3-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="335a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="335a3-127">Request body</span></span>
<span data-ttu-id="335a3-128">В тексте запроса добавьте представление объекта **денежных единиц** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="335a3-128">In the request body, supply a JSON representation of **currencies** object.</span></span>

## <a name="response"></a><span data-ttu-id="335a3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="335a3-129">Response</span></span>
<span data-ttu-id="335a3-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **валюты** в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="335a3-130">If successful, this method returns ```201 Created``` response code and a **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="335a3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="335a3-131">Example</span></span>

<span data-ttu-id="335a3-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="335a3-132">**Request**</span></span>

<span data-ttu-id="335a3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="335a3-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/currencies
Content-type: application/json

{
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01
}
```

<span data-ttu-id="335a3-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="335a3-134">**Response**</span></span>

<span data-ttu-id="335a3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="335a3-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="335a3-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="335a3-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="335a3-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="335a3-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:05:09.002Z"
}

```
