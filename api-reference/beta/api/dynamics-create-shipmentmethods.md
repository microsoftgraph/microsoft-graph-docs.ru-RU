---
title: Создание Шипментмесодс
description: Создает объект метода отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c59e690e33d847065c0e5c4a06ccbda0daeed2c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981608"
---
# <a name="create-shipmentmethods"></a><span data-ttu-id="9c3ac-103">Создание Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="9c3ac-103">Create shipmentMethods</span></span>

<span data-ttu-id="9c3ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c3ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c3ac-105">Создайте объект метода отгрузки в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-105">Create a shipment method object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c3ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c3ac-106">Permissions</span></span>
<span data-ttu-id="9c3ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c3ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c3ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c3ac-109">Permission type</span></span> |<span data-ttu-id="9c3ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c3ac-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9c3ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c3ac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c3ac-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c3ac-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9c3ac-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c3ac-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9c3ac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-114">Not supported.</span></span>|
|<span data-ttu-id="9c3ac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c3ac-115">Application</span></span>|<span data-ttu-id="9c3ac-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c3ac-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c3ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c3ac-117">HTTP request</span></span>
```
POST /financials/companies/{id}/shipmentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c3ac-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9c3ac-118">Optional query parameters</span></span>
<span data-ttu-id="9c3ac-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c3ac-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c3ac-120">Request headers</span></span>

|<span data-ttu-id="9c3ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c3ac-121">Header</span></span>         |<span data-ttu-id="9c3ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c3ac-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="9c3ac-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c3ac-123">Authorization</span></span>  |<span data-ttu-id="9c3ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9c3ac-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c3ac-126">Content-Type</span></span>   |<span data-ttu-id="9c3ac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9c3ac-127">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="9c3ac-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c3ac-128">Request body</span></span>
<span data-ttu-id="9c3ac-129">В тексте запроса добавьте представление объекта **шипментмесодс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-129">In the request body, supply a JSON representation of a **shipmentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="9c3ac-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c3ac-130">Response</span></span>
<span data-ttu-id="9c3ac-131">В случае успешного выполнения этот метод возвращает ```201 Created``` код отклика и объект **шипментмесодс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-131">If successful, this method returns ```201 Created``` response code and a **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c3ac-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9c3ac-132">Example</span></span>

<span data-ttu-id="9c3ac-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="9c3ac-133">**Request**</span></span>

<span data-ttu-id="9c3ac-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods
Content-type: application/json

{
  "code": "PICKUP",
  "displayName": "Pickup at Location"  
}
```

<span data-ttu-id="9c3ac-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="9c3ac-135">**Response**</span></span>

<span data-ttu-id="9c3ac-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="9c3ac-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9c3ac-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c3ac-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}

```


