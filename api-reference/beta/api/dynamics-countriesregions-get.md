---
title: Получение Каунтриесрегионс
description: Получает объект стран и регионов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 30916ec2fd6bd00f92a5ad96be05400d7ec4c92f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008389"
---
# <a name="get-countriesregions"></a><span data-ttu-id="f3a3b-103">Получение Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="f3a3b-103">Get countriesRegions</span></span>

<span data-ttu-id="f3a3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3a3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3a3b-105">Получение свойств и связей объекта Каунтриесрегионс для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-105">Retrieve the properties and relationships of a countriesRegions object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3a3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3a3b-106">Permissions</span></span>
<span data-ttu-id="f3a3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3a3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3a3b-109">Permission type</span></span> |<span data-ttu-id="f3a3b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3a3b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f3a3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3a3b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3a3b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a3b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f3a3b-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3a3b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f3a3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-114">Not supported.</span></span>|
|<span data-ttu-id="f3a3b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3a3b-115">Application</span></span>|<span data-ttu-id="f3a3b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a3b-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3a3b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3a3b-117">HTTP request</span></span>
```
GET /financials/companies/{id}/countriesRegions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3a3b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3a3b-118">Optional query parameters</span></span>
<span data-ttu-id="f3a3b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3a3b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3a3b-120">Request headers</span></span>
|<span data-ttu-id="f3a3b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3a3b-121">Header</span></span>|<span data-ttu-id="f3a3b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3a3b-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="f3a3b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3a3b-123">Authorization</span></span>  |<span data-ttu-id="f3a3b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3a3b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3a3b-126">Request body</span></span>
<span data-ttu-id="f3a3b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3a3b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3a3b-128">Response</span></span>
<span data-ttu-id="f3a3b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **каунтриесрегионс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-129">If successful, this method returns a `200 OK` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3a3b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f3a3b-130">Example</span></span>

<span data-ttu-id="f3a3b-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="f3a3b-131">**Request**</span></span>

<span data-ttu-id="f3a3b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions/{id}
```

<span data-ttu-id="f3a3b-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="f3a3b-133">**Response**</span></span>

<span data-ttu-id="f3a3b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="f3a3b-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f3a3b-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3a3b-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}
```


