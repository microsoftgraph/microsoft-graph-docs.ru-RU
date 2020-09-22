---
title: Получение Таксграупс
description: Получает метод групп налогов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 25e669956702cf8710b708e2fead1e26f80c8f74
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008108"
---
# <a name="get-taxgroups"></a><span data-ttu-id="68fc5-103">Получение Таксграупс</span><span class="sxs-lookup"><span data-stu-id="68fc5-103">Get taxGroups</span></span>

<span data-ttu-id="68fc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68fc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68fc5-105">Получение свойств и связей объекта налоговой группы для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="68fc5-105">Retrieve the properties and relationships of a tax groups object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="68fc5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68fc5-106">Permissions</span></span>
<span data-ttu-id="68fc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68fc5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68fc5-109">Permission type</span></span> |<span data-ttu-id="68fc5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68fc5-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="68fc5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68fc5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68fc5-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68fc5-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="68fc5-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68fc5-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="68fc5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68fc5-114">Not supported.</span></span>|
|<span data-ttu-id="68fc5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="68fc5-115">Application</span></span>|<span data-ttu-id="68fc5-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68fc5-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68fc5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68fc5-117">HTTP request</span></span>

```
GET /financials/companies/{id}/taxGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68fc5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68fc5-118">Optional query parameters</span></span>
<span data-ttu-id="68fc5-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="68fc5-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68fc5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68fc5-120">Request headers</span></span>
|<span data-ttu-id="68fc5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68fc5-121">Header</span></span>|<span data-ttu-id="68fc5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68fc5-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="68fc5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68fc5-123">Authorization</span></span>  |<span data-ttu-id="68fc5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68fc5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68fc5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68fc5-126">Request body</span></span>
<span data-ttu-id="68fc5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68fc5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68fc5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="68fc5-128">Response</span></span>
<span data-ttu-id="68fc5-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **таксграупс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68fc5-129">If successful, this method returns a `200 OK` response code and a **taxGroups** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68fc5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="68fc5-130">Example</span></span>

<span data-ttu-id="68fc5-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="68fc5-131">**Request**</span></span>

<span data-ttu-id="68fc5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68fc5-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/taxGroups/{id}
```

<span data-ttu-id="68fc5-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="68fc5-133">**Response**</span></span>

<span data-ttu-id="68fc5-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68fc5-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="68fc5-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="68fc5-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="68fc5-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68fc5-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}
```




