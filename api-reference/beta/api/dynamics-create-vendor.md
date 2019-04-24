---
title: Создание поставщиков
description: Создает объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 90c2c8a25602ac2a2c4197c916b9ce14e03b8e6d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458616"
---
# <a name="create-vendors"></a><span data-ttu-id="725c2-103">Создание поставщиков</span><span class="sxs-lookup"><span data-stu-id="725c2-103">Create vendors</span></span>
<span data-ttu-id="725c2-104">Создайте объект Vendor в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="725c2-104">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="725c2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="725c2-105">Permissions</span></span>
<span data-ttu-id="725c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="725c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="725c2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="725c2-108">Permission type</span></span> |<span data-ttu-id="725c2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="725c2-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="725c2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="725c2-110">Delegated (work or school account)</span></span>|<span data-ttu-id="725c2-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725c2-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="725c2-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="725c2-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="725c2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="725c2-113">Not supported.</span></span>|
|<span data-ttu-id="725c2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="725c2-114">Application</span></span>|<span data-ttu-id="725c2-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725c2-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="725c2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="725c2-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="725c2-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="725c2-117">Optional query parameters</span></span>
<span data-ttu-id="725c2-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="725c2-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="725c2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="725c2-119">Request headers</span></span>
|<span data-ttu-id="725c2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="725c2-120">Header</span></span>|<span data-ttu-id="725c2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="725c2-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="725c2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="725c2-122">Authorization</span></span>  |<span data-ttu-id="725c2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="725c2-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="725c2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="725c2-125">Content-Type</span></span>  |<span data-ttu-id="725c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="725c2-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="725c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="725c2-127">Request body</span></span>
<span data-ttu-id="725c2-128">В тексте запроса добавьте представление объекта вендоров в формате \*\*\*\* JSON.</span><span class="sxs-lookup"><span data-stu-id="725c2-128">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="725c2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="725c2-129">Response</span></span>
<span data-ttu-id="725c2-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **вендоров** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="725c2-130">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="725c2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="725c2-131">Example</span></span>

<span data-ttu-id="725c2-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="725c2-132">**Request**</span></span>

<span data-ttu-id="725c2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="725c2-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/vendors
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

<span data-ttu-id="725c2-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="725c2-134">**Response**</span></span>

<span data-ttu-id="725c2-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="725c2-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="725c2-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="725c2-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="725c2-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="725c2-137">All the properties will be returned from an actual call.</span></span>

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

