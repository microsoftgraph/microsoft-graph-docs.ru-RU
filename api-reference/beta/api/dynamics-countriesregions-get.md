---
title: Get countriesRegions
description: Получает объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 678151c8c03de09a1e72d7ce15bb1e8e7bf82b60
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473389"
---
# <a name="get-countriesregions"></a><span data-ttu-id="3d739-103">Get countriesRegions</span><span class="sxs-lookup"><span data-stu-id="3d739-103">Get countriesRegions</span></span>

<span data-ttu-id="3d739-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d739-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d739-105">Извлечение свойств и связей объекта countriesRegions для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="3d739-105">Retrieve the properties and relationships of a countriesRegions object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d739-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d739-106">Permissions</span></span>
<span data-ttu-id="3d739-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d739-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d739-109">Permission type</span></span> |<span data-ttu-id="3d739-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d739-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3d739-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d739-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d739-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d739-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3d739-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d739-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3d739-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d739-114">Not supported.</span></span>|
|<span data-ttu-id="3d739-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d739-115">Application</span></span>|<span data-ttu-id="3d739-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d739-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d739-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d739-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/countriesRegions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d739-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3d739-118">Optional query parameters</span></span>
<span data-ttu-id="3d739-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3d739-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d739-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d739-120">Request headers</span></span>
|<span data-ttu-id="3d739-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d739-121">Header</span></span>|<span data-ttu-id="3d739-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d739-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="3d739-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d739-123">Authorization</span></span>  |<span data-ttu-id="3d739-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d739-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d739-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d739-126">Request body</span></span>
<span data-ttu-id="3d739-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d739-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d739-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d739-128">Response</span></span>
<span data-ttu-id="3d739-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` **объект countriesRegions** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3d739-129">If successful, this method returns a `200 OK` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d739-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3d739-130">Example</span></span>

<span data-ttu-id="3d739-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="3d739-131">**Request**</span></span>

<span data-ttu-id="3d739-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d739-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions/{id}
```

<span data-ttu-id="3d739-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="3d739-133">**Response**</span></span>

<span data-ttu-id="3d739-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3d739-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="3d739-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3d739-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3d739-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d739-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}
```


