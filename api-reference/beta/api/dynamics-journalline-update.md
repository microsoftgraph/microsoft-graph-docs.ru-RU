---
title: Обновление journalLines
description: Обновляет строку журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 548bac42e1c46247858bcf18a21c0886fd5774df
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474332"
---
# <a name="update-journallines"></a><span data-ttu-id="16ef3-103">Обновление journalLines</span><span class="sxs-lookup"><span data-stu-id="16ef3-103">Update journalLines</span></span>

<span data-ttu-id="16ef3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16ef3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16ef3-105">Обновление свойств объекта строк журнала для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="16ef3-105">Update the properties of a journal lines object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="16ef3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16ef3-106">Permissions</span></span>
<span data-ttu-id="16ef3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16ef3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16ef3-109">Permission type</span></span> |<span data-ttu-id="16ef3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16ef3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="16ef3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16ef3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16ef3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16ef3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="16ef3-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16ef3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="16ef3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16ef3-114">Not supported.</span></span>|
|<span data-ttu-id="16ef3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16ef3-115">Application</span></span>|<span data-ttu-id="16ef3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16ef3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16ef3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16ef3-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16ef3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16ef3-118">Optional query parameters</span></span>
<span data-ttu-id="16ef3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16ef3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16ef3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16ef3-120">Request headers</span></span>
| <span data-ttu-id="16ef3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16ef3-121">Header</span></span>       | <span data-ttu-id="16ef3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16ef3-122">Value</span></span>                    |
|--------------|--------------------------|
|<span data-ttu-id="16ef3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16ef3-123">Authorization</span></span> |<span data-ttu-id="16ef3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16ef3-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="16ef3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16ef3-126">Content-Type</span></span>  |<span data-ttu-id="16ef3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="16ef3-127">application/json</span></span>          |
|<span data-ttu-id="16ef3-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="16ef3-128">If-Match</span></span>      |<span data-ttu-id="16ef3-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="16ef3-129">Required.</span></span> <span data-ttu-id="16ef3-130">Если заголовка запроса включена, а предоставленный eTag не соответствует текущему тегу в **journalLines,** **journalLines** не будет обновляться.</span><span class="sxs-lookup"><span data-stu-id="16ef3-130">When this request header is included and the eTag provided does not match the current tag on the **journalLines**, the **journalLines** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16ef3-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16ef3-131">Request body</span></span>
<span data-ttu-id="16ef3-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="16ef3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="16ef3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="16ef3-135">Response</span></span>
<span data-ttu-id="16ef3-136">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` **journalLines** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="16ef3-136">If successful, this method returns a `200 OK` response code and an updated **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16ef3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="16ef3-137">Example</span></span>

<span data-ttu-id="16ef3-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="16ef3-138">**Request**</span></span>

<span data-ttu-id="16ef3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16ef3-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines/{id}
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="16ef3-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="16ef3-140">**Response**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "",
  "accountNumber": "",
  "postingDate": "2015-12-31",
  "documentNumber": "D00001",
  "externalDocumentNumber": "",
  "amount": 2000,
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```




