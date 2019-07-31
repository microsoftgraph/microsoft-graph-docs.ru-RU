---
title: Удаление Шипментмесодс
description: Удаляет объект метода отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: fbe39b0727648f3e8a9226fb9650afc9f73b826c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956011"
---
# <a name="delete-shipmentmethods"></a><span data-ttu-id="ab228-103">Удаление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="ab228-103">Delete shipmentMethods</span></span>
<span data-ttu-id="ab228-104">Удаление объекта метода отгрузки из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="ab228-104">Delete a shipment method object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab228-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab228-105">Permissions</span></span>
<span data-ttu-id="ab228-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab228-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab228-108">Permission type</span></span> |<span data-ttu-id="ab228-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab228-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ab228-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab228-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ab228-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab228-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ab228-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab228-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ab228-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab228-113">Not supported.</span></span>|
|<span data-ttu-id="ab228-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab228-114">Application</span></span>|<span data-ttu-id="ab228-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab228-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab228-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab228-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/shipmentMethods('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab228-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab228-117">Optional query parameters</span></span>
<span data-ttu-id="ab228-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ab228-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab228-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab228-119">Request headers</span></span>
|<span data-ttu-id="ab228-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab228-120">Header</span></span>|<span data-ttu-id="ab228-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ab228-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="ab228-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab228-122">Authorization</span></span>  |<span data-ttu-id="ab228-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab228-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="ab228-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="ab228-125">If-Match</span></span>       |<span data-ttu-id="ab228-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ab228-126">Required.</span></span> <span data-ttu-id="ab228-127">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **шипментмесодс**, **шипментмесодс** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="ab228-127">When this request header is included and the eTag provided does not match the current tag on the **shipmentMethods**, the **shipmentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab228-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab228-128">Request body</span></span>
<span data-ttu-id="ab228-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab228-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab228-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab228-130">Response</span></span>
<span data-ttu-id="ab228-p104">В случае успешного выполнения этот метод возвращает код отклика ```204,No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ab228-p104">If successful, this method returns ```204,No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab228-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ab228-133">Example</span></span>

<span data-ttu-id="ab228-134">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="ab228-134">**Request**</span></span>

<span data-ttu-id="ab228-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab228-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/shipmentMethods('{id}')
```

<span data-ttu-id="ab228-136">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="ab228-136">**Response**</span></span> 

<span data-ttu-id="ab228-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ab228-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
