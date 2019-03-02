---
title: Создание Шипментмесодс
description: Создает объект метода отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4f83c186adf72dde6f88082db1a6156ebc7b12af
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365817"
---
# <a name="create-shipmentmethods"></a><span data-ttu-id="77758-103">Создание Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="77758-103">Create shipmentMethods</span></span>
<span data-ttu-id="77758-104">Создайте объект метода отгрузки в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="77758-104">Create a shipment method object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="77758-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77758-105">Permissions</span></span>
<span data-ttu-id="77758-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77758-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77758-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77758-108">Permission type</span></span> |<span data-ttu-id="77758-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77758-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="77758-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77758-110">Delegated (work or school account)</span></span>|<span data-ttu-id="77758-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77758-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="77758-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77758-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="77758-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77758-113">Not supported.</span></span>|
|<span data-ttu-id="77758-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77758-114">Application</span></span>|<span data-ttu-id="77758-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77758-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77758-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77758-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/shipmentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77758-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77758-117">Optional query parameters</span></span>
<span data-ttu-id="77758-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77758-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77758-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77758-119">Request headers</span></span>

|<span data-ttu-id="77758-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77758-120">Header</span></span>         |<span data-ttu-id="77758-121">Значение</span><span class="sxs-lookup"><span data-stu-id="77758-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="77758-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77758-122">Authorization</span></span>  |<span data-ttu-id="77758-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77758-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="77758-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77758-125">Content-Type</span></span>   |<span data-ttu-id="77758-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77758-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="77758-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77758-127">Request body</span></span>
<span data-ttu-id="77758-128">В тексте запроса добавьте представление объекта **Шипментмесодс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77758-128">In the request body, supply a JSON representation of a **shipmentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="77758-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="77758-129">Response</span></span>
<span data-ttu-id="77758-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **шипментмесодс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77758-130">If successful, this method returns ```201 Created``` response code and a **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77758-131">Пример</span><span class="sxs-lookup"><span data-stu-id="77758-131">Example</span></span>

<span data-ttu-id="77758-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="77758-132">**Request**</span></span>

<span data-ttu-id="77758-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77758-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/shipmentMethods
Content-type: application/json

{
  "code": "PICKUP",
  "displayName": "Pickup at Location"  
}
```

<span data-ttu-id="77758-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="77758-134">**Response**</span></span>

<span data-ttu-id="77758-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77758-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="77758-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="77758-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="77758-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77758-137">All the properties will be returned from an actual call.</span></span>

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
