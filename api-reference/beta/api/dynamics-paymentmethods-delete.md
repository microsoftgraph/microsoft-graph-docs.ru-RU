---
title: Удаление Пайментмесодс
description: Удаляет объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: a15fd1e1e07db00342391817ee204501bb7b196c
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791416"
---
# <a name="delete-paymentmethods"></a><span data-ttu-id="07c9c-103">Удаление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="07c9c-103">Delete paymentMethods</span></span>
<span data-ttu-id="07c9c-104">Удаление объекта метода оплаты из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="07c9c-104">Delete a payment method object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="07c9c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07c9c-105">Permissions</span></span>
<span data-ttu-id="07c9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c9c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07c9c-108">Permission type</span></span> |<span data-ttu-id="07c9c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07c9c-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="07c9c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07c9c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="07c9c-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c9c-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="07c9c-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07c9c-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="07c9c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c9c-113">Not supported.</span></span>|
|<span data-ttu-id="07c9c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07c9c-114">Application</span></span>|<span data-ttu-id="07c9c-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c9c-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c9c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07c9c-116">HTTP request</span></span>
```
DELETE /financials/companies/{id}/paymentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07c9c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07c9c-117">Optional query parameters</span></span>
<span data-ttu-id="07c9c-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07c9c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07c9c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07c9c-119">Request headers</span></span>

|<span data-ttu-id="07c9c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07c9c-120">Header</span></span>         |<span data-ttu-id="07c9c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="07c9c-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="07c9c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07c9c-122">Authorization</span></span>  |<span data-ttu-id="07c9c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07c9c-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="07c9c-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="07c9c-125">If-Match</span></span>       |<span data-ttu-id="07c9c-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="07c9c-126">Required.</span></span> <span data-ttu-id="07c9c-127">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **пайментмесодс**, **пайментмесодс** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="07c9c-127">When this request header is included and the eTag provided does not match the current tag on the **paymentMethods**, the **paymentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07c9c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07c9c-128">Request body</span></span>
<span data-ttu-id="07c9c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07c9c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07c9c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="07c9c-130">Response</span></span>
<span data-ttu-id="07c9c-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="07c9c-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07c9c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="07c9c-133">Example</span></span>

<span data-ttu-id="07c9c-134">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="07c9c-134">**Request**</span></span>

<span data-ttu-id="07c9c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07c9c-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods/{id}
```

<span data-ttu-id="07c9c-136">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="07c9c-136">**Response**</span></span> 

<span data-ttu-id="07c9c-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07c9c-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```

