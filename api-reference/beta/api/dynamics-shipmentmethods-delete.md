---
title: Удаление Шипментмесодс
description: Удаляет объект метода отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ebb4eb14f10f92458a6c83b8bc23b6e1cb506528
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42428476"
---
# <a name="delete-shipmentmethods"></a><span data-ttu-id="4ea4b-103">Удаление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="4ea4b-103">Delete shipmentMethods</span></span>

<span data-ttu-id="4ea4b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ea4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea4b-105">Удаление объекта метода отгрузки из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-105">Delete a shipment method object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ea4b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ea4b-106">Permissions</span></span>
<span data-ttu-id="4ea4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea4b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ea4b-109">Permission type</span></span> |<span data-ttu-id="4ea4b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ea4b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4ea4b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ea4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ea4b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea4b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4ea4b-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ea4b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4ea4b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-114">Not supported.</span></span>|
|<span data-ttu-id="4ea4b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ea4b-115">Application</span></span>|<span data-ttu-id="4ea4b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea4b-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ea4b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ea4b-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/shipmentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ea4b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ea4b-118">Optional query parameters</span></span>
<span data-ttu-id="4ea4b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ea4b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ea4b-120">Request headers</span></span>
|<span data-ttu-id="4ea4b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ea4b-121">Header</span></span>|<span data-ttu-id="4ea4b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4ea4b-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="4ea4b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ea4b-123">Authorization</span></span>  |<span data-ttu-id="4ea4b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="4ea4b-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="4ea4b-126">If-Match</span></span>       |<span data-ttu-id="4ea4b-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-127">Required.</span></span> <span data-ttu-id="4ea4b-128">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **шипментмесодс**, **шипментмесодс** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-128">When this request header is included and the eTag provided does not match the current tag on the **shipmentMethods**, the **shipmentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ea4b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ea4b-129">Request body</span></span>
<span data-ttu-id="4ea4b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ea4b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ea4b-131">Response</span></span>
<span data-ttu-id="4ea4b-p104">В случае успешного выполнения этот метод возвращает код отклика ```204,No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-p104">If successful, this method returns ```204,No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea4b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="4ea4b-134">Example</span></span>

<span data-ttu-id="4ea4b-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="4ea4b-135">**Request**</span></span>

<span data-ttu-id="4ea4b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods/{id}
```

<span data-ttu-id="4ea4b-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="4ea4b-137">**Response**</span></span> 

<span data-ttu-id="4ea4b-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ea4b-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
