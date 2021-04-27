---
title: Создание поставщиков
description: Создает объект поставщика в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 24e058f673e499aa58bf2c52765dc0c391412c07
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045686"
---
# <a name="create-vendors"></a><span data-ttu-id="f634c-103">Создание поставщиков</span><span class="sxs-lookup"><span data-stu-id="f634c-103">Create vendors</span></span>

<span data-ttu-id="f634c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f634c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f634c-105">Создание объекта поставщика в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f634c-105">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f634c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f634c-106">Permissions</span></span>
<span data-ttu-id="f634c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f634c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f634c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f634c-109">Permission type</span></span> |<span data-ttu-id="f634c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f634c-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f634c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f634c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f634c-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f634c-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f634c-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f634c-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f634c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f634c-114">Not supported.</span></span>|
|<span data-ttu-id="f634c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f634c-115">Application</span></span>|<span data-ttu-id="f634c-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f634c-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f634c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f634c-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f634c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f634c-118">Optional query parameters</span></span>
<span data-ttu-id="f634c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f634c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f634c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f634c-120">Request headers</span></span>
|<span data-ttu-id="f634c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f634c-121">Header</span></span>|<span data-ttu-id="f634c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f634c-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="f634c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f634c-123">Authorization</span></span>  |<span data-ttu-id="f634c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f634c-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f634c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f634c-126">Content-Type</span></span>  |<span data-ttu-id="f634c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f634c-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="f634c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f634c-128">Request body</span></span>
<span data-ttu-id="f634c-129">В теле запроса поставляем представление JSON объекта **поставщиков.**</span><span class="sxs-lookup"><span data-stu-id="f634c-129">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="f634c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f634c-130">Response</span></span>
<span data-ttu-id="f634c-131">В случае успешной работы этот метод возвращает код ответа и объект ```201 Created``` поставщиков в  тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f634c-131">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f634c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f634c-132">Example</span></span>

<span data-ttu-id="f634c-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="f634c-133">**Request**</span></span>

<span data-ttu-id="f634c-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f634c-134">Here is an example of a request.</span></span>

```http
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

<span data-ttu-id="f634c-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="f634c-135">**Response**</span></span>

<span data-ttu-id="f634c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f634c-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="f634c-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f634c-137">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```



