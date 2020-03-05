---
title: Создание Кустомерпайментжаурналс
description: Создает объект журнала платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: bf6b88ec992734114de7e63e82d97026b22f7081
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431622"
---
# <a name="create-customerpaymentjournals"></a><span data-ttu-id="7a410-103">Создание Кустомерпайментжаурналс</span><span class="sxs-lookup"><span data-stu-id="7a410-103">Create customerPaymentJournals</span></span>

<span data-ttu-id="7a410-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7a410-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a410-105">Создает объект журнала клиентских платежей в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="7a410-105">Creates a customer payment journal object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a410-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a410-106">Permissions</span></span>
<span data-ttu-id="7a410-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a410-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a410-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a410-109">Permission type</span></span> |<span data-ttu-id="7a410-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a410-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7a410-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a410-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a410-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a410-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7a410-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a410-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7a410-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a410-114">Not supported.</span></span>|
|<span data-ttu-id="7a410-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a410-115">Application</span></span>|<span data-ttu-id="7a410-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a410-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a410-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a410-117">HTTP request</span></span>

```
POST /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a410-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a410-118">Optional query parameters</span></span>
<span data-ttu-id="7a410-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7a410-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a410-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a410-120">Request headers</span></span>
|<span data-ttu-id="7a410-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a410-121">Header</span></span>        |<span data-ttu-id="7a410-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a410-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="7a410-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a410-123">Authorization</span></span> |<span data-ttu-id="7a410-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a410-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7a410-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a410-126">Content-Type</span></span>  |<span data-ttu-id="7a410-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7a410-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="7a410-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a410-128">Request body</span></span>
<span data-ttu-id="7a410-129">В тексте запроса добавьте представление объекта **кустомерпайментжаурналс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a410-129">In the request body, supply a JSON representation of **customerPaymentJournals** object.</span></span>

## <a name="response"></a><span data-ttu-id="7a410-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a410-130">Response</span></span>
<span data-ttu-id="7a410-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **кустомерпайментжаурналс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a410-131">If successful, this method returns ```201 Created``` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a410-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7a410-132">Example</span></span>

<span data-ttu-id="7a410-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="7a410-133">**Request**</span></span>

<span data-ttu-id="7a410-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a410-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="7a410-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="7a410-135">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


