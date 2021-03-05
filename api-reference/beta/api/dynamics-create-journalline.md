---
title: Создание journalLines
description: Создает строку журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 38feb577f11f482fe00c5d44d883e1b0995ff562
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473268"
---
# <a name="create-journallines"></a><span data-ttu-id="b103f-103">Создание journalLines</span><span class="sxs-lookup"><span data-stu-id="b103f-103">Create journalLines</span></span>

<span data-ttu-id="b103f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b103f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b103f-105">Создает объект строки журнала в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b103f-105">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b103f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b103f-106">Permissions</span></span>
<span data-ttu-id="b103f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b103f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b103f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b103f-109">Permission type</span></span> |<span data-ttu-id="b103f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b103f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b103f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b103f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b103f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b103f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b103f-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b103f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b103f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b103f-114">Not supported.</span></span>|
|<span data-ttu-id="b103f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b103f-115">Application</span></span>|<span data-ttu-id="b103f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b103f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b103f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b103f-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b103f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b103f-118">Optional query parameters</span></span>
<span data-ttu-id="b103f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b103f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b103f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b103f-120">Request headers</span></span>
|<span data-ttu-id="b103f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b103f-121">Header</span></span>        |<span data-ttu-id="b103f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b103f-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="b103f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b103f-123">Authorization</span></span> |<span data-ttu-id="b103f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b103f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b103f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b103f-126">Content-Type</span></span>  |<span data-ttu-id="b103f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b103f-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="b103f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b103f-128">Request body</span></span>
<span data-ttu-id="b103f-129">В теле запроса поставляем представление JSON объекта **journalLines.**</span><span class="sxs-lookup"><span data-stu-id="b103f-129">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="b103f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b103f-130">Response</span></span>
<span data-ttu-id="b103f-131">В случае успешной работы этот метод возвращает код отклика и ```201 Created``` **объект journalLines** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b103f-131">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b103f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b103f-132">Example</span></span>

<span data-ttu-id="b103f-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="b103f-133">**Request**</span></span>

<span data-ttu-id="b103f-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b103f-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines
Content-type: application/json

{
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": ""
}
```
<span data-ttu-id="b103f-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="b103f-135">**Response**</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```




