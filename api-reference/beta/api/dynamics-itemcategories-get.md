---
title: Get itemCategories
description: Получает категорию элементов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 489a9e8ce8f828e4ebd3b1538c885b07dcfe0fbe
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045268"
---
# <a name="get-itemcategories"></a><span data-ttu-id="ebabf-103">Get itemCategories</span><span class="sxs-lookup"><span data-stu-id="ebabf-103">Get itemCategories</span></span>

<span data-ttu-id="ebabf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebabf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebabf-105">Извлечение свойств и связей объекта категории элементов для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="ebabf-105">Retrieve the properties and relationships of an item category object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebabf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebabf-106">Permissions</span></span>
<span data-ttu-id="ebabf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebabf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebabf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebabf-109">Permission type</span></span> |<span data-ttu-id="ebabf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebabf-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ebabf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebabf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ebabf-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebabf-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ebabf-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebabf-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ebabf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebabf-114">Not supported.</span></span>|
|<span data-ttu-id="ebabf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebabf-115">Application</span></span>|<span data-ttu-id="ebabf-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebabf-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebabf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebabf-117">HTTP request</span></span>

```
GET /financials/companies/{id}/itemCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ebabf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ebabf-118">Optional query parameters</span></span>
<span data-ttu-id="ebabf-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ebabf-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebabf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebabf-120">Request headers</span></span>
|<span data-ttu-id="ebabf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebabf-121">Header</span></span>       |<span data-ttu-id="ebabf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ebabf-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="ebabf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebabf-123">Authorization</span></span>|<span data-ttu-id="ebabf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebabf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebabf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebabf-126">Request body</span></span>
<span data-ttu-id="ebabf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebabf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebabf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebabf-128">Response</span></span>
<span data-ttu-id="ebabf-129">В случае успеха этот метод возвращает код ответа и `200 OK` **объект itemCategories** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ebabf-129">If successful, this method returns a `200 OK` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebabf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ebabf-130">Example</span></span>

<span data-ttu-id="ebabf-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="ebabf-131">**Request**</span></span>

<span data-ttu-id="ebabf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebabf-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories/{id}
```

<span data-ttu-id="ebabf-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="ebabf-133">**Response**</span></span>

<span data-ttu-id="ebabf-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ebabf-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="ebabf-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ebabf-135">**Note**: The response object shown here might be shortened for readability.</span></span>

```json
{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}
```



