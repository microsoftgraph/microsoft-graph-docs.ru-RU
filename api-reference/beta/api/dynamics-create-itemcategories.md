---
title: Создание itemCategories
description: Создает объект категории элементов в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b50c1c9221c41c0e2bdb7cf5f24b4fbdd6ba9b13
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471357"
---
# <a name="create-itemcategories"></a><span data-ttu-id="0b7b5-103">Создание itemCategories</span><span class="sxs-lookup"><span data-stu-id="0b7b5-103">Create itemCategories</span></span>

<span data-ttu-id="0b7b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b7b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b7b5-105">Создание объекта категории элементов Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-105">Create an item category object Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b7b5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b7b5-106">Permissions</span></span>
<span data-ttu-id="0b7b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b7b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b7b5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b7b5-109">Permission type</span></span> |<span data-ttu-id="0b7b5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b7b5-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="0b7b5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b7b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b7b5-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b7b5-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="0b7b5-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b7b5-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0b7b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-114">Not supported.</span></span>|
|<span data-ttu-id="0b7b5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b7b5-115">Application</span></span>|<span data-ttu-id="0b7b5-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b7b5-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b7b5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b7b5-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/itemCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b7b5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b7b5-118">Optional query parameters</span></span>
<span data-ttu-id="0b7b5-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b7b5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b7b5-120">Request headers</span></span>
|<span data-ttu-id="0b7b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b7b5-121">Header</span></span>       |<span data-ttu-id="0b7b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b7b5-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="0b7b5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b7b5-123">Authorization</span></span>|<span data-ttu-id="0b7b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0b7b5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b7b5-126">Content-Type</span></span> |<span data-ttu-id="0b7b5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0b7b5-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="0b7b5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b7b5-128">Request body</span></span>
<span data-ttu-id="0b7b5-129">В теле запроса поставляем представление JSON объекта **itemCategories.**</span><span class="sxs-lookup"><span data-stu-id="0b7b5-129">In the request body, supply a JSON representation of an **itemCategories** object.</span></span>

## <a name="response"></a><span data-ttu-id="0b7b5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b7b5-130">Response</span></span>
<span data-ttu-id="0b7b5-131">В случае успеха этот метод возвращает код ответа и ```201 Created``` **объект itemCategories** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-131">If successful, this method returns ```201 Created``` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b7b5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0b7b5-132">Example</span></span>

<span data-ttu-id="0b7b5-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="0b7b5-133">**Request**</span></span>

<span data-ttu-id="0b7b5-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

<span data-ttu-id="0b7b5-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="0b7b5-135">**Response**</span></span>

<span data-ttu-id="0b7b5-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="0b7b5-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b7b5-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b7b5-138">All the properties will be returned from an actual call.</span></span>

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






