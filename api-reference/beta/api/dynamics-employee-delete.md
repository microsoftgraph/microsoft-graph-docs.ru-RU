---
title: Удаление сотрудников
description: Удаляет объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 47e9902bc51c739446cb9bf3055c063632cc7206
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981347"
---
# <a name="delete-employees"></a><span data-ttu-id="1843f-103">Удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="1843f-103">Delete employees</span></span>

<span data-ttu-id="1843f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1843f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1843f-105">Удаление сотрудника из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="1843f-105">Delete an employee from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="1843f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1843f-106">Permissions</span></span>
<span data-ttu-id="1843f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1843f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1843f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1843f-109">Permission type</span></span> |<span data-ttu-id="1843f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1843f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="1843f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1843f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1843f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1843f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="1843f-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1843f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1843f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1843f-114">Not supported.</span></span>|
|<span data-ttu-id="1843f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1843f-115">Application</span></span>|<span data-ttu-id="1843f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1843f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1843f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1843f-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1843f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1843f-118">Optional query parameters</span></span>
<span data-ttu-id="1843f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1843f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1843f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1843f-120">Request headers</span></span>
|<span data-ttu-id="1843f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1843f-121">Header</span></span>         |<span data-ttu-id="1843f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1843f-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="1843f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1843f-123">Authorization</span></span>  |<span data-ttu-id="1843f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1843f-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1843f-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="1843f-126">If-Match</span></span>       |<span data-ttu-id="1843f-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1843f-127">Required.</span></span> <span data-ttu-id="1843f-128">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу **сотрудников**, **сотрудники** не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="1843f-128">When this request header is included and the eTag provided does not match the current tag on the **employees**, the **employees** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1843f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1843f-129">Request body</span></span>
<span data-ttu-id="1843f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1843f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1843f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1843f-131">Response</span></span>
<span data-ttu-id="1843f-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1843f-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1843f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1843f-134">Example</span></span>

<span data-ttu-id="1843f-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="1843f-135">**Request**</span></span>

<span data-ttu-id="1843f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1843f-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
```

<span data-ttu-id="1843f-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="1843f-137">**Response**</span></span> 

<span data-ttu-id="1843f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1843f-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```



