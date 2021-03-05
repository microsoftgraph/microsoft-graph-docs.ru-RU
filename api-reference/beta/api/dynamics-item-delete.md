---
title: Удаление элементов
description: Удаляет объект элемента в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 76f498cbc5e8edfab73dc26735b10b46c6cbcee9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471278"
---
# <a name="delete-items"></a><span data-ttu-id="97b35-103">Удаление элементов</span><span class="sxs-lookup"><span data-stu-id="97b35-103">Delete items</span></span>

<span data-ttu-id="97b35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97b35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97b35-105">Удаление элемента из Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="97b35-105">Delete an item from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="97b35-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97b35-106">Permissions</span></span>
<span data-ttu-id="97b35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97b35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97b35-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97b35-109">Permission type</span></span> |<span data-ttu-id="97b35-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97b35-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="97b35-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97b35-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97b35-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b35-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="97b35-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97b35-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="97b35-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97b35-114">Not supported.</span></span>|
|<span data-ttu-id="97b35-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97b35-115">Application</span></span>|<span data-ttu-id="97b35-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b35-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97b35-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97b35-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/items/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97b35-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="97b35-118">Optional query parameters</span></span>
<span data-ttu-id="97b35-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="97b35-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97b35-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97b35-120">Request headers</span></span>
|<span data-ttu-id="97b35-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97b35-121">Header</span></span>       |<span data-ttu-id="97b35-122">Значение</span><span class="sxs-lookup"><span data-stu-id="97b35-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="97b35-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97b35-123">Authorization</span></span>|<span data-ttu-id="97b35-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97b35-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="97b35-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="97b35-126">If-Match</span></span>     |<span data-ttu-id="97b35-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="97b35-127">Required.</span></span> <span data-ttu-id="97b35-128">Если этот заглавный элемент запроса включен и предоставленный eTag  не соответствует текущему тегу элементов, элементы не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="97b35-128">When this request header is included and the eTag provided does not match the current tag on the **items**, the **items** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97b35-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97b35-129">Request body</span></span>
<span data-ttu-id="97b35-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97b35-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97b35-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="97b35-131">Response</span></span>
<span data-ttu-id="97b35-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="97b35-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97b35-134">Пример</span><span class="sxs-lookup"><span data-stu-id="97b35-134">Example</span></span>

<span data-ttu-id="97b35-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="97b35-135">**Request**</span></span>

<span data-ttu-id="97b35-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97b35-136">Here is an example of the request.</span></span>
```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/items/{id}
```

<span data-ttu-id="97b35-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="97b35-137">**Response**</span></span>

<span data-ttu-id="97b35-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97b35-138">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```



