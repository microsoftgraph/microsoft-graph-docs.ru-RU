---
title: Удаление валют
description: Удаляет объект валюты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b9f6c729dc97d523952454978afc056c05c354c5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473156"
---
# <a name="delete-currencies"></a><span data-ttu-id="23d99-103">Удаление валют</span><span class="sxs-lookup"><span data-stu-id="23d99-103">Delete currencies</span></span>

<span data-ttu-id="23d99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23d99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23d99-105">Удаление объекта валюты из Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="23d99-105">Delete a currency object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="23d99-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23d99-106">Permissions</span></span>
<span data-ttu-id="23d99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23d99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23d99-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23d99-109">Permission type</span></span> |<span data-ttu-id="23d99-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23d99-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="23d99-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23d99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="23d99-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23d99-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="23d99-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23d99-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="23d99-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23d99-114">Not supported.</span></span>|
|<span data-ttu-id="23d99-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23d99-115">Application</span></span>|<span data-ttu-id="23d99-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23d99-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23d99-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23d99-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23d99-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23d99-118">Optional query parameters</span></span>
<span data-ttu-id="23d99-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23d99-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23d99-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23d99-120">Request headers</span></span>

|<span data-ttu-id="23d99-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23d99-121">Header</span></span>|<span data-ttu-id="23d99-122">Значение</span><span class="sxs-lookup"><span data-stu-id="23d99-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="23d99-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23d99-123">Authorization</span></span>  |<span data-ttu-id="23d99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23d99-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="23d99-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="23d99-126">If-Match</span></span>       |<span data-ttu-id="23d99-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="23d99-127">Required.</span></span> <span data-ttu-id="23d99-128">При включении этого загона запроса и предоставленного eTag не  совпадает с текущим тегом в валютах, валюты не будут</span><span class="sxs-lookup"><span data-stu-id="23d99-128">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be</span></span>
 <span data-ttu-id="23d99-129">обновлено.</span><span class="sxs-lookup"><span data-stu-id="23d99-129">updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23d99-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23d99-130">Request body</span></span>
<span data-ttu-id="23d99-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23d99-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23d99-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="23d99-132">Response</span></span>
<span data-ttu-id="23d99-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="23d99-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23d99-135">Пример</span><span class="sxs-lookup"><span data-stu-id="23d99-135">Example</span></span>

<span data-ttu-id="23d99-136">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="23d99-136">**Request**</span></span>

<span data-ttu-id="23d99-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23d99-137">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

<span data-ttu-id="23d99-138">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="23d99-138">**Response**</span></span> 

<span data-ttu-id="23d99-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23d99-139">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```


