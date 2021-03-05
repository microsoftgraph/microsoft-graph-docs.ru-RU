---
title: Создание paymentMethods
description: Создает объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 64d7dac3590845f4fa4a95de9fc32829654a1d57
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473282"
---
# <a name="create-paymentmethods"></a><span data-ttu-id="7bede-103">Создание paymentMethods</span><span class="sxs-lookup"><span data-stu-id="7bede-103">Create paymentMethods</span></span>

<span data-ttu-id="7bede-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bede-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bede-105">Создание объекта метода оплаты в центре бизнеса DDynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7bede-105">Create a payment method object in DDynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bede-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bede-106">Permissions</span></span>
<span data-ttu-id="7bede-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bede-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bede-109">Permission type</span></span> |<span data-ttu-id="7bede-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bede-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7bede-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bede-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7bede-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bede-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7bede-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bede-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7bede-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bede-114">Not supported.</span></span>|
|<span data-ttu-id="7bede-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bede-115">Application</span></span>|<span data-ttu-id="7bede-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bede-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bede-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bede-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/paymentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bede-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7bede-118">Optional query parameters</span></span>
<span data-ttu-id="7bede-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7bede-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bede-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bede-120">Request headers</span></span>
|<span data-ttu-id="7bede-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bede-121">Header</span></span>         |<span data-ttu-id="7bede-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7bede-122">Value</span></span>                        |
|---------------|-----------------------------|
|<span data-ttu-id="7bede-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bede-123">Authorization</span></span>  |<span data-ttu-id="7bede-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bede-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="7bede-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bede-126">Content-Type</span></span>   |<span data-ttu-id="7bede-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7bede-127">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="7bede-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bede-128">Request body</span></span>
<span data-ttu-id="7bede-129">В теле запроса поставляем представление JSON объекта **paymentMethods.**</span><span class="sxs-lookup"><span data-stu-id="7bede-129">In the request body, supply a JSON representation of a **paymentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="7bede-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bede-130">Response</span></span>
<span data-ttu-id="7bede-131">В случае успешной работы этот метод возвращает код ответа и объект ```201 Created``` **paymentMethods** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7bede-131">If successful, this method returns ```201 Created``` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bede-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7bede-132">Example</span></span>

<span data-ttu-id="7bede-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="7bede-133">**Request**</span></span>

<span data-ttu-id="7bede-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bede-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
}
```

<span data-ttu-id="7bede-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="7bede-135">**Response**</span></span>

<span data-ttu-id="7bede-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7bede-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="7bede-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7bede-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7bede-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7bede-138">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}

```



