---
title: Удаление Пайментмесодс
description: Удаляет объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b5e65e596cdf53d20b117c39c2b4e7a3b63ce417
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42428756"
---
# <a name="delete-paymentmethods"></a><span data-ttu-id="eda3d-103">Удаление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="eda3d-103">Delete paymentMethods</span></span>

<span data-ttu-id="eda3d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eda3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eda3d-105">Удаление объекта метода оплаты из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="eda3d-105">Delete a payment method object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="eda3d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eda3d-106">Permissions</span></span>
<span data-ttu-id="eda3d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda3d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eda3d-109">Permission type</span></span> |<span data-ttu-id="eda3d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eda3d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="eda3d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eda3d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eda3d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda3d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="eda3d-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eda3d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="eda3d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda3d-114">Not supported.</span></span>|
|<span data-ttu-id="eda3d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eda3d-115">Application</span></span>|<span data-ttu-id="eda3d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda3d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda3d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eda3d-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/paymentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eda3d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eda3d-118">Optional query parameters</span></span>
<span data-ttu-id="eda3d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eda3d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eda3d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eda3d-120">Request headers</span></span>

|<span data-ttu-id="eda3d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eda3d-121">Header</span></span>         |<span data-ttu-id="eda3d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eda3d-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="eda3d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eda3d-123">Authorization</span></span>  |<span data-ttu-id="eda3d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eda3d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="eda3d-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="eda3d-126">If-Match</span></span>       |<span data-ttu-id="eda3d-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="eda3d-127">Required.</span></span> <span data-ttu-id="eda3d-128">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **пайментмесодс**, **пайментмесодс** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="eda3d-128">When this request header is included and the eTag provided does not match the current tag on the **paymentMethods**, the **paymentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eda3d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eda3d-129">Request body</span></span>
<span data-ttu-id="eda3d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eda3d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eda3d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="eda3d-131">Response</span></span>
<span data-ttu-id="eda3d-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="eda3d-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eda3d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="eda3d-134">Example</span></span>

<span data-ttu-id="eda3d-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="eda3d-135">**Request**</span></span>

<span data-ttu-id="eda3d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eda3d-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods/{id}
```

<span data-ttu-id="eda3d-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="eda3d-137">**Response**</span></span> 

<span data-ttu-id="eda3d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eda3d-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```

