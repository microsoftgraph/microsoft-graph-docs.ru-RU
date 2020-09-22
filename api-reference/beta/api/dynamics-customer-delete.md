---
title: Удаление клиентов
description: Удаляет объект Customers из Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 9dd3dd0d1a1938b02a339836aa410966043ca77d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981508"
---
# <a name="delete-customers"></a><span data-ttu-id="05212-103">Удаление клиентов</span><span class="sxs-lookup"><span data-stu-id="05212-103">Delete customers</span></span>

<span data-ttu-id="05212-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05212-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05212-105">Удаление объекта Customer из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="05212-105">Delete a customer object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="05212-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05212-106">Permissions</span></span>
<span data-ttu-id="05212-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05212-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05212-109">Permission type</span></span> |<span data-ttu-id="05212-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05212-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="05212-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05212-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05212-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05212-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="05212-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05212-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="05212-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05212-114">Not supported.</span></span>|
|<span data-ttu-id="05212-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05212-115">Application</span></span>|<span data-ttu-id="05212-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05212-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05212-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05212-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05212-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="05212-118">Optional query parameters</span></span>
<span data-ttu-id="05212-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="05212-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05212-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05212-120">Request headers</span></span>
|<span data-ttu-id="05212-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05212-121">Header</span></span>         |<span data-ttu-id="05212-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05212-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="05212-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05212-123">Authorization</span></span>  |<span data-ttu-id="05212-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05212-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="05212-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="05212-126">If-Match</span></span>       |<span data-ttu-id="05212-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="05212-127">Required.</span></span> <span data-ttu-id="05212-128">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу **клиентов**, **Клиенты** не будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="05212-128">When this request header is included and the eTag provided does not match the current tag on the **customers**, the **customers** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05212-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05212-129">Request body</span></span>
<span data-ttu-id="05212-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05212-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05212-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="05212-131">Response</span></span>
<span data-ttu-id="05212-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="05212-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05212-134">Пример</span><span class="sxs-lookup"><span data-stu-id="05212-134">Example</span></span>

<span data-ttu-id="05212-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="05212-135">**Request**</span></span>

<span data-ttu-id="05212-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05212-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
```

<span data-ttu-id="05212-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="05212-137">**Response**</span></span> 

<span data-ttu-id="05212-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05212-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```



