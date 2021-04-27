---
title: Создание itemCategories
description: Создает объект категории элементов в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 656da2b42c6af3234e1869a868eb87e755c2e916
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045889"
---
# <a name="create-itemcategories"></a><span data-ttu-id="81909-103">Создание itemCategories</span><span class="sxs-lookup"><span data-stu-id="81909-103">Create itemCategories</span></span>

<span data-ttu-id="81909-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81909-105">Создание объекта категории элементов Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="81909-105">Create an item category object Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="81909-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81909-106">Permissions</span></span>
<span data-ttu-id="81909-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81909-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81909-109">Permission type</span></span> |<span data-ttu-id="81909-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81909-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="81909-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81909-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81909-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81909-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="81909-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81909-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="81909-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81909-114">Not supported.</span></span>|
|<span data-ttu-id="81909-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81909-115">Application</span></span>|<span data-ttu-id="81909-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81909-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81909-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81909-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/itemCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81909-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81909-118">Optional query parameters</span></span>
<span data-ttu-id="81909-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81909-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81909-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81909-120">Request headers</span></span>
|<span data-ttu-id="81909-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81909-121">Header</span></span>       |<span data-ttu-id="81909-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81909-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="81909-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81909-123">Authorization</span></span>|<span data-ttu-id="81909-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81909-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="81909-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81909-126">Content-Type</span></span> |<span data-ttu-id="81909-127">application/json</span><span class="sxs-lookup"><span data-stu-id="81909-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="81909-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81909-128">Request body</span></span>
<span data-ttu-id="81909-129">В теле запроса поставляем представление JSON объекта **itemCategories.**</span><span class="sxs-lookup"><span data-stu-id="81909-129">In the request body, supply a JSON representation of an **itemCategories** object.</span></span>

## <a name="response"></a><span data-ttu-id="81909-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="81909-130">Response</span></span>
<span data-ttu-id="81909-131">В случае успеха этот метод возвращает код ответа и ```201 Created``` **объект itemCategories** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="81909-131">If successful, this method returns ```201 Created``` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81909-132">Пример</span><span class="sxs-lookup"><span data-stu-id="81909-132">Example</span></span>

<span data-ttu-id="81909-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="81909-133">**Request**</span></span>

<span data-ttu-id="81909-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81909-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

<span data-ttu-id="81909-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="81909-135">**Response**</span></span>

<span data-ttu-id="81909-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81909-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="81909-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="81909-137">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}

```






