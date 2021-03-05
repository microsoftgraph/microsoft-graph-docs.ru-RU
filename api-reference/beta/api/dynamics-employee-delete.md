---
title: Удаление сотрудников
description: Удаляет объект сотрудника в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f5aeab6c8b746ddd815ae26bf99e401c71d91746
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471279"
---
# <a name="delete-employees"></a><span data-ttu-id="ab5ba-103">Удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="ab5ba-103">Delete employees</span></span>

<span data-ttu-id="ab5ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab5ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab5ba-105">Удаление сотрудника из Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-105">Delete an employee from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab5ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab5ba-106">Permissions</span></span>
<span data-ttu-id="ab5ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab5ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab5ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab5ba-109">Permission type</span></span> |<span data-ttu-id="ab5ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab5ba-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ab5ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab5ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab5ba-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab5ba-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ab5ba-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab5ba-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ab5ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-114">Not supported.</span></span>|
|<span data-ttu-id="ab5ba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab5ba-115">Application</span></span>|<span data-ttu-id="ab5ba-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab5ba-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab5ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab5ba-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab5ba-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab5ba-118">Optional query parameters</span></span>
<span data-ttu-id="ab5ba-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab5ba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab5ba-120">Request headers</span></span>
|<span data-ttu-id="ab5ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab5ba-121">Header</span></span>         |<span data-ttu-id="ab5ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab5ba-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="ab5ba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab5ba-123">Authorization</span></span>  |<span data-ttu-id="ab5ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="ab5ba-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="ab5ba-126">If-Match</span></span>       |<span data-ttu-id="ab5ba-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-127">Required.</span></span> <span data-ttu-id="ab5ba-128">Если этот заглавный запрос включен и предоставленный eTag не соответствует  текущему тегу сотрудников, сотрудники не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-128">When this request header is included and the eTag provided does not match the current tag on the **employees**, the **employees** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab5ba-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab5ba-129">Request body</span></span>
<span data-ttu-id="ab5ba-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab5ba-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab5ba-131">Response</span></span>
<span data-ttu-id="ab5ba-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab5ba-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ab5ba-134">Example</span></span>

<span data-ttu-id="ab5ba-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="ab5ba-135">**Request**</span></span>

<span data-ttu-id="ab5ba-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-136">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
```

<span data-ttu-id="ab5ba-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="ab5ba-137">**Response**</span></span> 

<span data-ttu-id="ab5ba-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ab5ba-138">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```



