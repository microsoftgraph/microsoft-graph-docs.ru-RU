---
title: Обновление Пайментмесодс
description: Обновляет объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 28ce56d439b43e8706f3a726dc6f18d0b79c64bb
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791402"
---
# <a name="update-paymentmethods"></a><span data-ttu-id="274ce-103">Обновление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="274ce-103">Update paymentMethods</span></span>
<span data-ttu-id="274ce-104">Обновление свойств объекта метода оплаты для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="274ce-104">Update the properties of a payment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="274ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="274ce-105">Permissions</span></span>
<span data-ttu-id="274ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="274ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="274ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="274ce-108">Permission type</span></span> |<span data-ttu-id="274ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="274ce-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="274ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="274ce-110">Delegated (work or school account)</span></span>|<span data-ttu-id="274ce-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="274ce-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="274ce-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="274ce-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="274ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="274ce-113">Not supported.</span></span>|
|<span data-ttu-id="274ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="274ce-114">Application</span></span>|<span data-ttu-id="274ce-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="274ce-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="274ce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="274ce-116">HTTP request</span></span>
```
PATCH /financials/companies/{id}/paymentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="274ce-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="274ce-117">Optional query parameters</span></span>
<span data-ttu-id="274ce-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="274ce-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="274ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="274ce-119">Request headers</span></span>
|<span data-ttu-id="274ce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="274ce-120">Header</span></span>        |<span data-ttu-id="274ce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="274ce-121">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="274ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="274ce-122">Authorization</span></span> |<span data-ttu-id="274ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="274ce-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="274ce-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="274ce-125">Content-Type</span></span>  |<span data-ttu-id="274ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="274ce-126">application/json</span></span>          |
|<span data-ttu-id="274ce-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="274ce-127">If-Match</span></span>      |<span data-ttu-id="274ce-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="274ce-128">Required.</span></span> <span data-ttu-id="274ce-129">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **пайментмесодс**, **пайментмесодс** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="274ce-129">When this request header is included and the eTag provided does not match the current tag on the **paymentMethods**, the **paymentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="274ce-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="274ce-130">Request body</span></span>
<span data-ttu-id="274ce-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="274ce-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="274ce-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="274ce-134">Response</span></span>
<span data-ttu-id="274ce-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект **пайментмесодс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="274ce-135">If successful, this method returns a `200 OK` response code and an updated **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="274ce-136">Пример</span><span class="sxs-lookup"><span data-stu-id="274ce-136">Example</span></span>

<span data-ttu-id="274ce-137">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="274ce-137">**Request**</span></span>

<span data-ttu-id="274ce-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="274ce-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods/{id}
Content-type: application/json

{
  "displayName": "Personal Check Payment",
}
```

<span data-ttu-id="274ce-139">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="274ce-139">**Response**</span></span>

<span data-ttu-id="274ce-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="274ce-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="274ce-141">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="274ce-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="274ce-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="274ce-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Personal Check Payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}
```


