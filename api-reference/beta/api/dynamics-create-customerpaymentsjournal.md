---
title: Создание Кустомерпайментжаурналс
description: Создает объект журнала платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f24726931cd6aec7d4f246879bb3da32d23bdd3c
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792067"
---
# <a name="create-customerpaymentjournals"></a><span data-ttu-id="cca7b-103">Создание Кустомерпайментжаурналс</span><span class="sxs-lookup"><span data-stu-id="cca7b-103">Create customerPaymentJournals</span></span>
<span data-ttu-id="cca7b-104">Создает объект журнала клиентских платежей в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="cca7b-104">Creates a customer payment journal object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="cca7b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cca7b-105">Permissions</span></span>
<span data-ttu-id="cca7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cca7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cca7b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cca7b-108">Permission type</span></span> |<span data-ttu-id="cca7b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cca7b-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="cca7b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cca7b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="cca7b-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cca7b-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="cca7b-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cca7b-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cca7b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cca7b-113">Not supported.</span></span>|
|<span data-ttu-id="cca7b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cca7b-114">Application</span></span>|<span data-ttu-id="cca7b-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cca7b-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cca7b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cca7b-116">HTTP request</span></span>

```
POST /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cca7b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cca7b-117">Optional query parameters</span></span>
<span data-ttu-id="cca7b-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cca7b-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cca7b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cca7b-119">Request headers</span></span>
|<span data-ttu-id="cca7b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cca7b-120">Header</span></span>        |<span data-ttu-id="cca7b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cca7b-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="cca7b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cca7b-122">Authorization</span></span> |<span data-ttu-id="cca7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cca7b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cca7b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cca7b-125">Content-Type</span></span>  |<span data-ttu-id="cca7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cca7b-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="cca7b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cca7b-127">Request body</span></span>
<span data-ttu-id="cca7b-128">В тексте запроса добавьте представление объекта **кустомерпайментжаурналс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cca7b-128">In the request body, supply a JSON representation of **customerPaymentJournals** object.</span></span>

## <a name="response"></a><span data-ttu-id="cca7b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cca7b-129">Response</span></span>
<span data-ttu-id="cca7b-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **кустомерпайментжаурналс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cca7b-130">If successful, this method returns ```201 Created``` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cca7b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cca7b-131">Example</span></span>

<span data-ttu-id="cca7b-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="cca7b-132">**Request**</span></span>

<span data-ttu-id="cca7b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cca7b-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="cca7b-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="cca7b-134">**Response**</span></span>

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


