---
title: Обновление Таксареас
description: Обновляет объект налоговой области в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c6c3cedd16e8cca7a801d597718482ef1b6c12a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955927"
---
# <a name="update-taxareas"></a><span data-ttu-id="56cb8-103">Обновление Таксареас</span><span class="sxs-lookup"><span data-stu-id="56cb8-103">Update taxAreas</span></span>
<span data-ttu-id="56cb8-104">Обновление свойств объекта налоговой области для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="56cb8-104">Update the properties of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="56cb8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56cb8-105">Permissions</span></span>
<span data-ttu-id="56cb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56cb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56cb8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56cb8-108">Permission type</span></span> |<span data-ttu-id="56cb8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56cb8-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="56cb8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56cb8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="56cb8-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56cb8-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="56cb8-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56cb8-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="56cb8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56cb8-113">Not supported.</span></span>|
|<span data-ttu-id="56cb8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56cb8-114">Application</span></span>|<span data-ttu-id="56cb8-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56cb8-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56cb8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56cb8-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/taxAreas('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56cb8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="56cb8-117">Optional query parameters</span></span>
<span data-ttu-id="56cb8-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="56cb8-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56cb8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56cb8-119">Request headers</span></span>
|<span data-ttu-id="56cb8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56cb8-120">Header</span></span>|<span data-ttu-id="56cb8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="56cb8-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="56cb8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56cb8-122">Authorization</span></span> |<span data-ttu-id="56cb8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56cb8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="56cb8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56cb8-125">Content-Type</span></span>  |<span data-ttu-id="56cb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56cb8-126">application/json</span></span>|
|<span data-ttu-id="56cb8-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="56cb8-127">If-Match</span></span>      |<span data-ttu-id="56cb8-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="56cb8-128">Required.</span></span> <span data-ttu-id="56cb8-129">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **таксареас**, **таксареас** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="56cb8-129">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56cb8-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56cb8-130">Request body</span></span>
<span data-ttu-id="56cb8-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="56cb8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="56cb8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="56cb8-134">Response</span></span>
<span data-ttu-id="56cb8-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект **таксареас** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56cb8-135">If successful, this method returns a `200 OK` response code and an updated **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56cb8-136">Пример</span><span class="sxs-lookup"><span data-stu-id="56cb8-136">Example</span></span>

<span data-ttu-id="56cb8-137">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="56cb8-137">**Request**</span></span>

<span data-ttu-id="56cb8-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56cb8-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/taxAreas('{id}')
Content-type: application/json

{
  "code": "28012001T",
  "displayName": "tax area",
}
```

<span data-ttu-id="56cb8-139">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="56cb8-139">**Response**</span></span>

<span data-ttu-id="56cb8-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56cb8-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="56cb8-141">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="56cb8-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="56cb8-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56cb8-142">All the properties will be returned from an actual call.</span></span>

```json
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

