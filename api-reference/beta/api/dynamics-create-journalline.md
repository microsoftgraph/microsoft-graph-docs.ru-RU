---
title: Создание Жаурналлинес
description: Создает строку журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c0d047840143c87618eb33fc1ee9d0bc074f3f7e
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791955"
---
# <a name="create-journallines"></a><span data-ttu-id="e5be8-103">Создание Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="e5be8-103">Create journalLines</span></span>
<span data-ttu-id="e5be8-104">Создает объект строки журнала в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="e5be8-104">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5be8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5be8-105">Permissions</span></span>
<span data-ttu-id="e5be8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5be8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5be8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5be8-108">Permission type</span></span> |<span data-ttu-id="e5be8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5be8-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e5be8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5be8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e5be8-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5be8-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e5be8-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5be8-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e5be8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5be8-113">Not supported.</span></span>|
|<span data-ttu-id="e5be8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5be8-114">Application</span></span>|<span data-ttu-id="e5be8-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5be8-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5be8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5be8-116">HTTP request</span></span>

```
POST /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5be8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5be8-117">Optional query parameters</span></span>
<span data-ttu-id="e5be8-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5be8-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5be8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5be8-119">Request headers</span></span>
|<span data-ttu-id="e5be8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5be8-120">Header</span></span>        |<span data-ttu-id="e5be8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5be8-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="e5be8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5be8-122">Authorization</span></span> |<span data-ttu-id="e5be8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5be8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e5be8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5be8-125">Content-Type</span></span>  |<span data-ttu-id="e5be8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5be8-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="e5be8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5be8-127">Request body</span></span>
<span data-ttu-id="e5be8-128">В тексте запроса добавьте представление объекта **жаурналлинес** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5be8-128">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="e5be8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5be8-129">Response</span></span>
<span data-ttu-id="e5be8-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **жаурналлинес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5be8-130">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5be8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e5be8-131">Example</span></span>

<span data-ttu-id="e5be8-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="e5be8-132">**Request**</span></span>

<span data-ttu-id="e5be8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5be8-133">Here is an example of a request.</span></span>

```json
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
<span data-ttu-id="e5be8-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="e5be8-134">**Response**</span></span>

```json
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


