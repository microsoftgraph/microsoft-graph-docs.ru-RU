---
title: Удаление countriesRegions
description: Удаляет объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 7b1eb1b9f933663ce29cfa053a23621b27ef6b8e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473618"
---
# <a name="delete-countriesregions"></a><span data-ttu-id="91f1e-103">Удаление countriesRegions</span><span class="sxs-lookup"><span data-stu-id="91f1e-103">Delete countriesRegions</span></span>

<span data-ttu-id="91f1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91f1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91f1e-105">Удаление объекта стран и регионов из Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="91f1e-105">Delete a countries/regions object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="91f1e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91f1e-106">Permissions</span></span>
<span data-ttu-id="91f1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91f1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91f1e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91f1e-109">Permission type</span></span> |<span data-ttu-id="91f1e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91f1e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="91f1e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91f1e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91f1e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f1e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="91f1e-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91f1e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="91f1e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91f1e-114">Not supported.</span></span>|
|<span data-ttu-id="91f1e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91f1e-115">Application</span></span>|<span data-ttu-id="91f1e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f1e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91f1e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91f1e-117">HTTP request</span></span>
```http
DELETE /financials/companies/{id}/countriesRegions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91f1e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91f1e-118">Optional query parameters</span></span>
<span data-ttu-id="91f1e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91f1e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91f1e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91f1e-120">Request headers</span></span>
|<span data-ttu-id="91f1e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91f1e-121">Header</span></span>|<span data-ttu-id="91f1e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="91f1e-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="91f1e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91f1e-123">Authorization</span></span>  |<span data-ttu-id="91f1e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91f1e-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="91f1e-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="91f1e-126">If-Match</span></span>       |<span data-ttu-id="91f1e-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="91f1e-127">Required.</span></span> <span data-ttu-id="91f1e-128">Если этот заглавный запрос включен и предоставленный eTag не соответствует текущему тегу в **countriesRegions,** **страныRegions** не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="91f1e-128">When this request header is included and the eTag provided does not match the current tag on the **countriesRegions**, the **countriesRegions** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91f1e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91f1e-129">Request body</span></span>
<span data-ttu-id="91f1e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91f1e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91f1e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="91f1e-131">Response</span></span>
<span data-ttu-id="91f1e-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="91f1e-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f1e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="91f1e-134">Example</span></span>

<span data-ttu-id="91f1e-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="91f1e-135">**Request**</span></span>

<span data-ttu-id="91f1e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91f1e-136">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions/{id}
```

<span data-ttu-id="91f1e-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="91f1e-137">**Response**</span></span> 

<span data-ttu-id="91f1e-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91f1e-138">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```


