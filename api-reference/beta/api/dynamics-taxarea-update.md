---
title: Обновление taxAreas
description: Обновляет объект налоговых областей в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 5a191eda591291ce18411f78e62f525d470970ba
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044923"
---
# <a name="update-taxareas"></a><span data-ttu-id="d79a9-103">Обновление taxAreas</span><span class="sxs-lookup"><span data-stu-id="d79a9-103">Update taxAreas</span></span>

<span data-ttu-id="d79a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d79a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d79a9-105">Обновление свойств объекта области налогообложения для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="d79a9-105">Update the properties of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d79a9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d79a9-106">Permissions</span></span>
<span data-ttu-id="d79a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d79a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d79a9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d79a9-109">Permission type</span></span> |<span data-ttu-id="d79a9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d79a9-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d79a9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d79a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d79a9-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d79a9-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d79a9-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d79a9-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d79a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d79a9-114">Not supported.</span></span>|
|<span data-ttu-id="d79a9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d79a9-115">Application</span></span>|<span data-ttu-id="d79a9-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d79a9-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d79a9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d79a9-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d79a9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d79a9-118">Optional query parameters</span></span>
<span data-ttu-id="d79a9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d79a9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d79a9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d79a9-120">Request headers</span></span>
|<span data-ttu-id="d79a9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d79a9-121">Header</span></span>|<span data-ttu-id="d79a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d79a9-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="d79a9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d79a9-123">Authorization</span></span> |<span data-ttu-id="d79a9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d79a9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d79a9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d79a9-126">Content-Type</span></span>  |<span data-ttu-id="d79a9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d79a9-127">application/json</span></span>|
|<span data-ttu-id="d79a9-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="d79a9-128">If-Match</span></span>      |<span data-ttu-id="d79a9-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d79a9-129">Required.</span></span> <span data-ttu-id="d79a9-130">Если этот заглавный запрос включен и предоставленный eTag не соответствует текущему тегу **taxAreas,** **taxAreas** не будет обновляться.</span><span class="sxs-lookup"><span data-stu-id="d79a9-130">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d79a9-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d79a9-131">Request body</span></span>
<span data-ttu-id="d79a9-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d79a9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="d79a9-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d79a9-135">Response</span></span>
<span data-ttu-id="d79a9-136">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` **taxAreas** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d79a9-136">If successful, this method returns a `200 OK` response code and an updated **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d79a9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d79a9-137">Example</span></span>

<span data-ttu-id="d79a9-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d79a9-138">**Request**</span></span>

<span data-ttu-id="d79a9-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d79a9-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
Content-type: application/json

{
  "code": "28012001T",
  "displayName": "tax area",
}
```

<span data-ttu-id="d79a9-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d79a9-140">**Response**</span></span>

<span data-ttu-id="d79a9-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d79a9-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="d79a9-142">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d79a9-142">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



