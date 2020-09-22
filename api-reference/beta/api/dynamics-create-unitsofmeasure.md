---
title: Создание Унитсофмеасуре
description: Создает объект единицы измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 518e79afa8276c5ee94474dadb7b02e4eab4b1f6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981578"
---
# <a name="create-unitsofmeasure"></a><span data-ttu-id="13468-103">Создание Унитсофмеасуре</span><span class="sxs-lookup"><span data-stu-id="13468-103">Create unitsOfMeasure</span></span>

<span data-ttu-id="13468-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13468-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13468-105">Создайте объект единицы измерения в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="13468-105">Create a units of measure object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="13468-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13468-106">Permissions</span></span>
<span data-ttu-id="13468-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13468-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13468-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13468-109">Permission type</span></span> |<span data-ttu-id="13468-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13468-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="13468-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13468-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13468-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13468-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="13468-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13468-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="13468-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13468-114">Not supported.</span></span>|
|<span data-ttu-id="13468-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13468-115">Application</span></span>|<span data-ttu-id="13468-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13468-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13468-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13468-117">HTTP request</span></span>
```
POST /financials/companies/{id}/unitsOfMeasure
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13468-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13468-118">Optional query parameters</span></span>
<span data-ttu-id="13468-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="13468-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13468-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13468-120">Request headers</span></span>
|<span data-ttu-id="13468-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13468-121">Header</span></span>|<span data-ttu-id="13468-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13468-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="13468-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13468-123">Authorization</span></span>  |<span data-ttu-id="13468-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13468-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="13468-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13468-126">Content-Type</span></span>  |<span data-ttu-id="13468-127">application/json</span><span class="sxs-lookup"><span data-stu-id="13468-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="13468-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13468-128">Request body</span></span>
<span data-ttu-id="13468-129">В тексте запроса добавьте представление объекта **унитсофмеасуре** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13468-129">In the request body, supply a JSON representation of a **unitsOfMeasure** object.</span></span>

## <a name="response"></a><span data-ttu-id="13468-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="13468-130">Response</span></span>
<span data-ttu-id="13468-131">В случае успешного выполнения этот метод возвращает ```201 Created``` код отклика и объект **унитсофмеасуре** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13468-131">If successful, this method returns ```201 Created``` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13468-132">Пример</span><span class="sxs-lookup"><span data-stu-id="13468-132">Example</span></span>

<span data-ttu-id="13468-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="13468-133">**Request**</span></span>

<span data-ttu-id="13468-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13468-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure
Content-type: application/json

{
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA"
}
```

<span data-ttu-id="13468-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="13468-135">**Response**</span></span>

<span data-ttu-id="13468-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13468-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="13468-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="13468-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13468-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13468-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}

```



