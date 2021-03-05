---
title: Get generalLedgerEntries
description: Получает общий объект записи книги в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: d3862417cd75e2a6adb55c1c9660b8b1c2ddabc4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473051"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="ff8aa-103">Get generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="ff8aa-103">Get generalLedgerEntries</span></span>

<span data-ttu-id="ff8aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff8aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff8aa-105">Извлечение свойств и связей объекта записи общей книги для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-105">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff8aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff8aa-106">Permissions</span></span>
<span data-ttu-id="ff8aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff8aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff8aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff8aa-109">Permission type</span></span> |<span data-ttu-id="ff8aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff8aa-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ff8aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff8aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff8aa-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff8aa-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ff8aa-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff8aa-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ff8aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-114">Not supported.</span></span>|
|<span data-ttu-id="ff8aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff8aa-115">Application</span></span>|<span data-ttu-id="ff8aa-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff8aa-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="ff8aa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff8aa-117">HTTP request</span></span>
```
GET /financials/companies/{id}/generalLedgerEntries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff8aa-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff8aa-118">Optional query parameters</span></span>
<span data-ttu-id="ff8aa-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff8aa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff8aa-120">Request headers</span></span>
|<span data-ttu-id="ff8aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff8aa-121">Header</span></span>       |<span data-ttu-id="ff8aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff8aa-122">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="ff8aa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff8aa-123">Authorization</span></span>|<span data-ttu-id="ff8aa-124">Носителер.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-124">Bearer.</span></span> <span data-ttu-id="ff8aa-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff8aa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff8aa-126">Request body</span></span>
<span data-ttu-id="ff8aa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff8aa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff8aa-128">Response</span></span>
<span data-ttu-id="ff8aa-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` **объект generalLedgerEntries** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-129">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff8aa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ff8aa-130">Example</span></span>

<span data-ttu-id="ff8aa-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="ff8aa-131">**Request**</span></span>

<span data-ttu-id="ff8aa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/generalLedgerEntries/{id}
```

<span data-ttu-id="ff8aa-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="ff8aa-133">**Response**</span></span>

<span data-ttu-id="ff8aa-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="ff8aa-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff8aa-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff8aa-136">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "10700",
    "postingDate": "2017-03-15",
    "documentNumber": "108027",
    "documentType": "Invoice",
    "accountId": "id-value",
    "accountNumber": "7210",
    "description": "Order 106003",
    "debitAmount": 6943.8,
    "creditAmount": 0,
    "lastModifiedDateTime": "2017-03-15T02:20:58.747Z"
}
```



