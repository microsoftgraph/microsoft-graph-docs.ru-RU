---
title: Получение Унитсофмеасуре
description: Возвращает объект единицы измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 56030276c3d5cf0ce6a583dbb1fa82d41d996b93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008075"
---
# <a name="get-unitsofmeasure"></a><span data-ttu-id="018f0-103">Получение Унитсофмеасуре</span><span class="sxs-lookup"><span data-stu-id="018f0-103">Get unitsOfMeasure</span></span>

<span data-ttu-id="018f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="018f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="018f0-105">Получение свойств и связей объекта единиц измерения для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="018f0-105">Retrieve the properties and relationships of a units of measure object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="018f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="018f0-106">Permissions</span></span>
<span data-ttu-id="018f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="018f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="018f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="018f0-109">Permission type</span></span> |<span data-ttu-id="018f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="018f0-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="018f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="018f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="018f0-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018f0-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="018f0-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="018f0-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="018f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="018f0-114">Not supported.</span></span>|
|<span data-ttu-id="018f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="018f0-115">Application</span></span>|<span data-ttu-id="018f0-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018f0-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="018f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="018f0-117">HTTP request</span></span>

```
GET /financials/companies/{id}/unitsOfMeasure/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="018f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="018f0-118">Optional query parameters</span></span>
<span data-ttu-id="018f0-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="018f0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="018f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="018f0-120">Request headers</span></span>
|<span data-ttu-id="018f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="018f0-121">Header</span></span>|<span data-ttu-id="018f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="018f0-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="018f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="018f0-123">Authorization</span></span>  |<span data-ttu-id="018f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="018f0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="018f0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="018f0-126">Request body</span></span>
<span data-ttu-id="018f0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="018f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="018f0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="018f0-128">Response</span></span>
<span data-ttu-id="018f0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **унитсофмеасуре** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="018f0-129">If successful, this method returns a `200 OK` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="018f0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="018f0-130">Example</span></span>

<span data-ttu-id="018f0-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="018f0-131">**Request**</span></span>

<span data-ttu-id="018f0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="018f0-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure/{id}
```

<span data-ttu-id="018f0-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="018f0-133">**Response**</span></span>

<span data-ttu-id="018f0-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="018f0-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="018f0-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="018f0-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="018f0-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="018f0-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```


