---
title: Get paymentMethods
description: Получает объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b2162578856b80deff2507ccf97222cb825f61a1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474318"
---
# <a name="get-paymentmethods"></a><span data-ttu-id="7aa9e-103">Get paymentMethods</span><span class="sxs-lookup"><span data-stu-id="7aa9e-103">Get paymentMethods</span></span>

<span data-ttu-id="7aa9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aa9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aa9e-105">Извлечение свойств и связей объекта метода оплаты для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-105">Retrieve the properties and relationships of a payment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aa9e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7aa9e-106">Permissions</span></span>
<span data-ttu-id="7aa9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa9e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aa9e-109">Permission type</span></span> |<span data-ttu-id="7aa9e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aa9e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7aa9e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aa9e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7aa9e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa9e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7aa9e-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aa9e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7aa9e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-114">Not supported.</span></span>|
|<span data-ttu-id="7aa9e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7aa9e-115">Application</span></span>|<span data-ttu-id="7aa9e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa9e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aa9e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aa9e-117">HTTP request</span></span>

```
GET /financials/companies/{id}/paymentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7aa9e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7aa9e-118">Optional query parameters</span></span>
<span data-ttu-id="7aa9e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7aa9e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7aa9e-120">Request headers</span></span>
|<span data-ttu-id="7aa9e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7aa9e-121">Header</span></span>         |<span data-ttu-id="7aa9e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7aa9e-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="7aa9e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7aa9e-123">Authorization</span></span>  |<span data-ttu-id="7aa9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aa9e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7aa9e-126">Request body</span></span>
<span data-ttu-id="7aa9e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aa9e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aa9e-128">Response</span></span>
<span data-ttu-id="7aa9e-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` **paymentMethods** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-129">If successful, this method returns a `200 OK` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aa9e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7aa9e-130">Example</span></span>

<span data-ttu-id="7aa9e-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="7aa9e-131">**Request**</span></span>

<span data-ttu-id="7aa9e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods/{id}
```

<span data-ttu-id="7aa9e-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="7aa9e-133">**Response**</span></span>

<span data-ttu-id="7aa9e-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="7aa9e-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7aa9e-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7aa9e-136">All the properties will be returned from an actual call.</span></span>

```json
{

  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}
```




