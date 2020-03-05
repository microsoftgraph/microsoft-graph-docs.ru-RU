---
title: Обновление журналов
description: Обновляет объект журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: da1439a97fc540d9c22febff7ed3c2cf70861ec3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42429022"
---
# <a name="update-journals"></a><span data-ttu-id="e6b7b-103">Обновление журналов</span><span class="sxs-lookup"><span data-stu-id="e6b7b-103">Update journals</span></span>

<span data-ttu-id="e6b7b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e6b7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6b7b-105">Обновление свойств объекта журнала для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-105">Update the properties of a journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6b7b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6b7b-106">Permissions</span></span>
<span data-ttu-id="e6b7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6b7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6b7b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6b7b-109">Permission type</span></span> |<span data-ttu-id="e6b7b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6b7b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e6b7b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6b7b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6b7b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6b7b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e6b7b-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6b7b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e6b7b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-114">Not supported.</span></span>|
|<span data-ttu-id="e6b7b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6b7b-115">Application</span></span>|<span data-ttu-id="e6b7b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6b7b-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6b7b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6b7b-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6b7b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6b7b-118">Optional query parameters</span></span>
<span data-ttu-id="e6b7b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6b7b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6b7b-120">Request headers</span></span>
|<span data-ttu-id="e6b7b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6b7b-121">Header</span></span>        |<span data-ttu-id="e6b7b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e6b7b-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="e6b7b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6b7b-123">Authorization</span></span> |<span data-ttu-id="e6b7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e6b7b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6b7b-126">Content-Type</span></span>  |<span data-ttu-id="e6b7b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e6b7b-127">application/json</span></span>         |
|<span data-ttu-id="e6b7b-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="e6b7b-128">If-Match</span></span>      |<span data-ttu-id="e6b7b-129">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-129">Required.</span></span> <span data-ttu-id="e6b7b-130">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **журналах**, **журналы** не будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-130">When this request header is included and the eTag provided does not match the current tag on the **journals**, the **journals** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6b7b-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6b7b-131">Request body</span></span>
<span data-ttu-id="e6b7b-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="e6b7b-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6b7b-135">Response</span></span>
<span data-ttu-id="e6b7b-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект **журналов** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-136">If successful, this method returns a `200 OK` response code and an updated **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6b7b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e6b7b-137">Example</span></span>

<span data-ttu-id="e6b7b-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="e6b7b-138">**Request**</span></span>

<span data-ttu-id="e6b7b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}
Content-type: application/json

{
  "code": "EXPENSE",
  "displayName": "Expense Batch"
}
```

<span data-ttu-id="e6b7b-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="e6b7b-140">**Response**</span></span>

<span data-ttu-id="e6b7b-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="e6b7b-142">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e6b7b-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6b7b-143">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "EXPENSE",
  "displayName": "Expense Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

