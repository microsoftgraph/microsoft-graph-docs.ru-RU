---
title: Получение Женералледжерентриес
description: Возвращает объект записи главной книги в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 06884308987eb8010be965d30d09e064e3d67d5e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458511"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="6a1b2-103">Получение Женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="6a1b2-103">Get generalLedgerEntries</span></span>
<span data-ttu-id="6a1b2-104">Получение свойств и связей объекта записи главной книги для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-104">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a1b2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a1b2-105">Permissions</span></span>
<span data-ttu-id="6a1b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a1b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a1b2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a1b2-108">Permission type</span></span> |<span data-ttu-id="6a1b2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a1b2-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6a1b2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a1b2-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6a1b2-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a1b2-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6a1b2-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a1b2-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6a1b2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-113">Not supported.</span></span>|
|<span data-ttu-id="6a1b2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a1b2-114">Application</span></span>|<span data-ttu-id="6a1b2-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a1b2-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="6a1b2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a1b2-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/generalLedgerEntries('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a1b2-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a1b2-117">Optional query parameters</span></span>
<span data-ttu-id="6a1b2-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a1b2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a1b2-119">Request headers</span></span>
|<span data-ttu-id="6a1b2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a1b2-120">Header</span></span>       |<span data-ttu-id="6a1b2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6a1b2-121">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="6a1b2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a1b2-122">Authorization</span></span>|<span data-ttu-id="6a1b2-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-123">Bearer.</span></span> <span data-ttu-id="6a1b2-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a1b2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a1b2-125">Request body</span></span>
<span data-ttu-id="6a1b2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a1b2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a1b2-127">Response</span></span>
<span data-ttu-id="6a1b2-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **женералледжерентриес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-128">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a1b2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6a1b2-129">Example</span></span>

<span data-ttu-id="6a1b2-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="6a1b2-130">**Request**</span></span>

<span data-ttu-id="6a1b2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/generalLedgerEntries('{id}')
```

<span data-ttu-id="6a1b2-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="6a1b2-132">**Response**</span></span>

<span data-ttu-id="6a1b2-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="6a1b2-134">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6a1b2-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a1b2-135">All the properties will be returned from an actual call.</span></span>

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

