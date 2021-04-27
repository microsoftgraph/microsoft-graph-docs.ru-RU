---
title: Создание countriesRegions
description: Создает объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c220f8bf4bed00c5203921cfb4efde0d29105152
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046029"
---
# <a name="create-countriesregions"></a><span data-ttu-id="15058-103">Создание countriesRegions</span><span class="sxs-lookup"><span data-stu-id="15058-103">Create countriesRegions</span></span>

<span data-ttu-id="15058-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15058-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15058-105">Создание объекта countriesRegions в Центре бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="15058-105">Create a countriesRegions object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="15058-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15058-106">Permissions</span></span>
<span data-ttu-id="15058-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15058-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15058-109">Permission type</span></span> |<span data-ttu-id="15058-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15058-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="15058-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15058-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15058-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15058-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="15058-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15058-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="15058-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15058-114">Not supported.</span></span>|
|<span data-ttu-id="15058-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15058-115">Application</span></span>|<span data-ttu-id="15058-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15058-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15058-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15058-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/countriesRegions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15058-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15058-118">Optional query parameters</span></span>
<span data-ttu-id="15058-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15058-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15058-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15058-120">Request headers</span></span>
|<span data-ttu-id="15058-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15058-121">Header</span></span>|<span data-ttu-id="15058-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15058-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="15058-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15058-123">Authorization</span></span>  |<span data-ttu-id="15058-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15058-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="15058-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15058-126">Content-Type</span></span>  |<span data-ttu-id="15058-127">application/json</span><span class="sxs-lookup"><span data-stu-id="15058-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="15058-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15058-128">Request body</span></span>
<span data-ttu-id="15058-129">В теле запроса поставляем JSON-представление **объекта countriesRegions.**</span><span class="sxs-lookup"><span data-stu-id="15058-129">In the request body, supply a JSON representation of **countriesRegions** object.</span></span>

## <a name="response"></a><span data-ttu-id="15058-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="15058-130">Response</span></span>
<span data-ttu-id="15058-131">В случае успешной работы этот метод возвращает код ответа и ```201 Created``` **объект countriesRegions** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="15058-131">If successful, this method returns ```201 Created``` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15058-132">Пример</span><span class="sxs-lookup"><span data-stu-id="15058-132">Example</span></span>

<span data-ttu-id="15058-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="15058-133">**Request**</span></span>

<span data-ttu-id="15058-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15058-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions
Content-type: application/json

{
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code"
}
```

<span data-ttu-id="15058-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="15058-135">**Response**</span></span>

<span data-ttu-id="15058-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15058-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="15058-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="15058-137">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
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



