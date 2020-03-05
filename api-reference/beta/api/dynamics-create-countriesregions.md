---
title: Создание Каунтриесрегионс
description: Создает объект стран и регионов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 585907fd49981bacb7037fb13660dc18987ea1fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431846"
---
# <a name="create-countriesregions"></a><span data-ttu-id="e027a-103">Создание Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="e027a-103">Create countriesRegions</span></span>

<span data-ttu-id="e027a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e027a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e027a-105">Создание объекта Каунтриесрегионс в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="e027a-105">Create a countriesRegions object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e027a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e027a-106">Permissions</span></span>
<span data-ttu-id="e027a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e027a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e027a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e027a-109">Permission type</span></span> |<span data-ttu-id="e027a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e027a-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e027a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e027a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e027a-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e027a-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e027a-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e027a-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e027a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e027a-114">Not supported.</span></span>|
|<span data-ttu-id="e027a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e027a-115">Application</span></span>|<span data-ttu-id="e027a-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e027a-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e027a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e027a-117">HTTP request</span></span>
```
POST /financials/companies/{id}/countriesRegions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e027a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e027a-118">Optional query parameters</span></span>
<span data-ttu-id="e027a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e027a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e027a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e027a-120">Request headers</span></span>
|<span data-ttu-id="e027a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e027a-121">Header</span></span>|<span data-ttu-id="e027a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e027a-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="e027a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e027a-123">Authorization</span></span>  |<span data-ttu-id="e027a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e027a-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e027a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e027a-126">Content-Type</span></span>  |<span data-ttu-id="e027a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e027a-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="e027a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e027a-128">Request body</span></span>
<span data-ttu-id="e027a-129">В тексте запроса добавьте представление объекта **каунтриесрегионс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e027a-129">In the request body, supply a JSON representation of **countriesRegions** object.</span></span>

## <a name="response"></a><span data-ttu-id="e027a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e027a-130">Response</span></span>
<span data-ttu-id="e027a-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **каунтриесрегионс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e027a-131">If successful, this method returns ```201 Created``` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e027a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e027a-132">Example</span></span>

<span data-ttu-id="e027a-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="e027a-133">**Request**</span></span>

<span data-ttu-id="e027a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e027a-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions
Content-type: application/json

{
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code"
}
```

<span data-ttu-id="e027a-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="e027a-135">**Response**</span></span>

<span data-ttu-id="e027a-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e027a-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="e027a-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e027a-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e027a-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e027a-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}

```

