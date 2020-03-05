---
title: Получение Каунтриесрегионс
description: Получает объект стран и регионов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: d916ed3e1de5643983808c3bd410a2746d64c2b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431902"
---
# <a name="get-countriesregions"></a><span data-ttu-id="e6051-103">Получение Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="e6051-103">Get countriesRegions</span></span>

<span data-ttu-id="e6051-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e6051-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6051-105">Получение свойств и связей объекта Каунтриесрегионс для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="e6051-105">Retrieve the properties and relationships of a countriesRegions object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6051-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6051-106">Permissions</span></span>
<span data-ttu-id="e6051-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6051-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6051-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6051-109">Permission type</span></span> |<span data-ttu-id="e6051-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6051-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e6051-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6051-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6051-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6051-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e6051-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6051-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e6051-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6051-114">Not supported.</span></span>|
|<span data-ttu-id="e6051-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6051-115">Application</span></span>|<span data-ttu-id="e6051-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6051-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6051-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6051-117">HTTP request</span></span>
```
GET /financials/companies/{id}/countriesRegions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6051-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6051-118">Optional query parameters</span></span>
<span data-ttu-id="e6051-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6051-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6051-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6051-120">Request headers</span></span>
|<span data-ttu-id="e6051-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6051-121">Header</span></span>|<span data-ttu-id="e6051-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e6051-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="e6051-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6051-123">Authorization</span></span>  |<span data-ttu-id="e6051-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6051-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6051-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6051-126">Request body</span></span>
<span data-ttu-id="e6051-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6051-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6051-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6051-128">Response</span></span>
<span data-ttu-id="e6051-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **каунтриесрегионс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6051-129">If successful, this method returns a `200 OK` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6051-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e6051-130">Example</span></span>

<span data-ttu-id="e6051-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="e6051-131">**Request**</span></span>

<span data-ttu-id="e6051-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6051-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions/{id}
```

<span data-ttu-id="e6051-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="e6051-133">**Response**</span></span>

<span data-ttu-id="e6051-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e6051-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="e6051-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e6051-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e6051-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6051-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}
```
