---
title: Удаление пересылкиМетходы
description: Удаляет объект метода отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b22a2eae6afe5cec579a54e1d42050169570ced7
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474255"
---
# <a name="delete-shipmentmethods"></a><span data-ttu-id="c4aa9-103">Удаление пересылкиМетходы</span><span class="sxs-lookup"><span data-stu-id="c4aa9-103">Delete shipmentMethods</span></span>

<span data-ttu-id="c4aa9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4aa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4aa9-105">Удаление объекта метода отгрузки из Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-105">Delete a shipment method object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4aa9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4aa9-106">Permissions</span></span>
<span data-ttu-id="c4aa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4aa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4aa9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4aa9-109">Permission type</span></span> |<span data-ttu-id="c4aa9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4aa9-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c4aa9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4aa9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4aa9-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4aa9-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c4aa9-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4aa9-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c4aa9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-114">Not supported.</span></span>|
|<span data-ttu-id="c4aa9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4aa9-115">Application</span></span>|<span data-ttu-id="c4aa9-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4aa9-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4aa9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4aa9-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/shipmentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4aa9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4aa9-118">Optional query parameters</span></span>
<span data-ttu-id="c4aa9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4aa9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4aa9-120">Request headers</span></span>
|<span data-ttu-id="c4aa9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4aa9-121">Header</span></span>|<span data-ttu-id="c4aa9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c4aa9-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="c4aa9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4aa9-123">Authorization</span></span>  |<span data-ttu-id="c4aa9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c4aa9-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="c4aa9-126">If-Match</span></span>       |<span data-ttu-id="c4aa9-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-127">Required.</span></span> <span data-ttu-id="c4aa9-128">Если этот загон запроса включен и предоставленный eTag не совпадает с текущим тегом на **пересылкеMethods,** **отправкаMethods** не будет обновляться.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-128">When this request header is included and the eTag provided does not match the current tag on the **shipmentMethods**, the **shipmentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4aa9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4aa9-129">Request body</span></span>
<span data-ttu-id="c4aa9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4aa9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4aa9-131">Response</span></span>
<span data-ttu-id="c4aa9-p104">В случае успешного выполнения этот метод возвращает код отклика ```204,No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-p104">If successful, this method returns ```204,No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4aa9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c4aa9-134">Example</span></span>

<span data-ttu-id="c4aa9-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="c4aa9-135">**Request**</span></span>

<span data-ttu-id="c4aa9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-136">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods/{id}
```

<span data-ttu-id="c4aa9-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="c4aa9-137">**Response**</span></span> 

<span data-ttu-id="c4aa9-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4aa9-138">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```


