---
title: Создание Итемкатегориес
description: Создает объект категории элемента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3ecf5df6dbd03014ba026ba8673c9a4b2fffd5b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431482"
---
# <a name="create-itemcategories"></a><span data-ttu-id="b8c92-103">Создание Итемкатегориес</span><span class="sxs-lookup"><span data-stu-id="b8c92-103">Create itemCategories</span></span>

<span data-ttu-id="b8c92-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b8c92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8c92-105">Создайте объект категории элемента Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b8c92-105">Create an item category object Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8c92-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8c92-106">Permissions</span></span>
<span data-ttu-id="b8c92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8c92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8c92-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8c92-109">Permission type</span></span> |<span data-ttu-id="b8c92-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8c92-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b8c92-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8c92-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8c92-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8c92-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b8c92-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8c92-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b8c92-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8c92-114">Not supported.</span></span>|
|<span data-ttu-id="b8c92-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8c92-115">Application</span></span>|<span data-ttu-id="b8c92-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8c92-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8c92-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8c92-117">HTTP request</span></span>
```
POST /financials/companies/{id}/itemCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8c92-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8c92-118">Optional query parameters</span></span>
<span data-ttu-id="b8c92-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b8c92-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8c92-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8c92-120">Request headers</span></span>
|<span data-ttu-id="b8c92-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8c92-121">Header</span></span>       |<span data-ttu-id="b8c92-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b8c92-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="b8c92-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8c92-123">Authorization</span></span>|<span data-ttu-id="b8c92-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8c92-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b8c92-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8c92-126">Content-Type</span></span> |<span data-ttu-id="b8c92-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b8c92-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="b8c92-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8c92-128">Request body</span></span>
<span data-ttu-id="b8c92-129">В тексте запроса добавьте представление объекта **итемкатегориес** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8c92-129">In the request body, supply a JSON representation of an **itemCategories** object.</span></span>

## <a name="response"></a><span data-ttu-id="b8c92-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8c92-130">Response</span></span>
<span data-ttu-id="b8c92-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **итемкатегориес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8c92-131">If successful, this method returns ```201 Created``` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8c92-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b8c92-132">Example</span></span>

<span data-ttu-id="b8c92-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="b8c92-133">**Request**</span></span>

<span data-ttu-id="b8c92-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8c92-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

<span data-ttu-id="b8c92-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="b8c92-135">**Response**</span></span>

<span data-ttu-id="b8c92-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8c92-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="b8c92-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b8c92-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8c92-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8c92-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}

```




