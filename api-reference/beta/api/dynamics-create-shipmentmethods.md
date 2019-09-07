---
title: Создание Шипментмесодс
description: Создает объект метода отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4c9ce592c2cc24aa9cac0731b678c473a9c18447
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791941"
---
# <a name="create-shipmentmethods"></a><span data-ttu-id="05f56-103">Создание Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="05f56-103">Create shipmentMethods</span></span>
<span data-ttu-id="05f56-104">Создайте объект метода отгрузки в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="05f56-104">Create a shipment method object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="05f56-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05f56-105">Permissions</span></span>
<span data-ttu-id="05f56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05f56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05f56-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05f56-108">Permission type</span></span> |<span data-ttu-id="05f56-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05f56-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="05f56-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05f56-110">Delegated (work or school account)</span></span>|<span data-ttu-id="05f56-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05f56-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="05f56-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05f56-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="05f56-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f56-113">Not supported.</span></span>|
|<span data-ttu-id="05f56-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05f56-114">Application</span></span>|<span data-ttu-id="05f56-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05f56-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05f56-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05f56-116">HTTP request</span></span>
```
POST /financials/companies/{id}/shipmentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05f56-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="05f56-117">Optional query parameters</span></span>
<span data-ttu-id="05f56-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="05f56-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05f56-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05f56-119">Request headers</span></span>

|<span data-ttu-id="05f56-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05f56-120">Header</span></span>         |<span data-ttu-id="05f56-121">Значение</span><span class="sxs-lookup"><span data-stu-id="05f56-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="05f56-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05f56-122">Authorization</span></span>  |<span data-ttu-id="05f56-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05f56-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="05f56-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05f56-125">Content-Type</span></span>   |<span data-ttu-id="05f56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05f56-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="05f56-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05f56-127">Request body</span></span>
<span data-ttu-id="05f56-128">В тексте запроса добавьте представление объекта **шипментмесодс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05f56-128">In the request body, supply a JSON representation of a **shipmentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="05f56-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="05f56-129">Response</span></span>
<span data-ttu-id="05f56-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **шипментмесодс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05f56-130">If successful, this method returns ```201 Created``` response code and a **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05f56-131">Пример</span><span class="sxs-lookup"><span data-stu-id="05f56-131">Example</span></span>

<span data-ttu-id="05f56-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="05f56-132">**Request**</span></span>

<span data-ttu-id="05f56-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05f56-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods
Content-type: application/json

{
  "code": "PICKUP",
  "displayName": "Pickup at Location"  
}
```

<span data-ttu-id="05f56-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="05f56-134">**Response**</span></span>

<span data-ttu-id="05f56-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05f56-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="05f56-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="05f56-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="05f56-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05f56-137">All the properties will be returned from an actual call.</span></span>

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
