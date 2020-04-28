---
title: Создание поставщиков
description: Создает объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2bf393a954078585cc89a073947c636a233a2a00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431087"
---
# <a name="create-vendors"></a><span data-ttu-id="cde4d-103">Создание поставщиков</span><span class="sxs-lookup"><span data-stu-id="cde4d-103">Create vendors</span></span>

<span data-ttu-id="cde4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cde4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cde4d-105">Создайте объект Vendor в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="cde4d-105">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="cde4d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cde4d-106">Permissions</span></span>
<span data-ttu-id="cde4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cde4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cde4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cde4d-109">Permission type</span></span> |<span data-ttu-id="cde4d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cde4d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="cde4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cde4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cde4d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cde4d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="cde4d-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cde4d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cde4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde4d-114">Not supported.</span></span>|
|<span data-ttu-id="cde4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cde4d-115">Application</span></span>|<span data-ttu-id="cde4d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cde4d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cde4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cde4d-117">HTTP request</span></span>
```
POST /financials/companies/{id}/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cde4d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cde4d-118">Optional query parameters</span></span>
<span data-ttu-id="cde4d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cde4d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cde4d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cde4d-120">Request headers</span></span>
|<span data-ttu-id="cde4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cde4d-121">Header</span></span>|<span data-ttu-id="cde4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cde4d-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="cde4d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cde4d-123">Authorization</span></span>  |<span data-ttu-id="cde4d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cde4d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="cde4d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cde4d-126">Content-Type</span></span>  |<span data-ttu-id="cde4d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cde4d-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="cde4d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cde4d-128">Request body</span></span>
<span data-ttu-id="cde4d-129">В тексте запроса добавьте представление объекта **вендоров** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cde4d-129">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="cde4d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cde4d-130">Response</span></span>
<span data-ttu-id="cde4d-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **вендоров** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cde4d-131">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cde4d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cde4d-132">Example</span></span>

<span data-ttu-id="cde4d-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="cde4d-133">**Request**</span></span>

<span data-ttu-id="cde4d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cde4d-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/vendors
Content-type: application/json

{
  "number": "40000",
  "displayName": "Wide World Importers",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "irs1099Code": "",
  "taxLiable": true,
  "blocked": " "
}
```

<span data-ttu-id="cde4d-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="cde4d-135">**Response**</span></span>

<span data-ttu-id="cde4d-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cde4d-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="cde4d-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cde4d-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cde4d-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cde4d-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}

```

