---
title: Удаление валют
description: Удаляет объект Currency в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ce3980118a26276ab712e2c422b9260b8624b31c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956515"
---
# <a name="delete-currencies"></a><span data-ttu-id="f0798-103">Удаление валют</span><span class="sxs-lookup"><span data-stu-id="f0798-103">Delete currencies</span></span>
<span data-ttu-id="f0798-104">Удаление объекта Currency из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f0798-104">Delete a currency object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0798-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0798-105">Permissions</span></span>
<span data-ttu-id="f0798-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0798-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0798-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0798-108">Permission type</span></span> |<span data-ttu-id="f0798-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0798-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f0798-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0798-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f0798-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0798-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f0798-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0798-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f0798-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0798-113">Not supported.</span></span>|
|<span data-ttu-id="f0798-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0798-114">Application</span></span>|<span data-ttu-id="f0798-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0798-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0798-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0798-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/currencies('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0798-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0798-117">Optional query parameters</span></span>
<span data-ttu-id="f0798-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f0798-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0798-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0798-119">Request headers</span></span>

|<span data-ttu-id="f0798-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0798-120">Header</span></span>|<span data-ttu-id="f0798-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f0798-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="f0798-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0798-122">Authorization</span></span>  |<span data-ttu-id="f0798-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0798-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f0798-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="f0798-125">If-Match</span></span>       |<span data-ttu-id="f0798-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f0798-126">Required.</span></span> <span data-ttu-id="f0798-127">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **валютах**, то **валюты** не будут</span><span class="sxs-lookup"><span data-stu-id="f0798-127">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be</span></span>
 <span data-ttu-id="f0798-128">обновленный.</span><span class="sxs-lookup"><span data-stu-id="f0798-128">updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0798-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0798-129">Request body</span></span>
<span data-ttu-id="f0798-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0798-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0798-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0798-131">Response</span></span>
<span data-ttu-id="f0798-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f0798-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0798-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f0798-134">Example</span></span>

<span data-ttu-id="f0798-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="f0798-135">**Request**</span></span>

<span data-ttu-id="f0798-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0798-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/currencies('{id}')
```

<span data-ttu-id="f0798-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="f0798-137">**Response**</span></span> 

<span data-ttu-id="f0798-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0798-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
