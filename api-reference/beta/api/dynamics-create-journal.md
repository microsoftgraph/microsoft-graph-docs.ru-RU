---
title: Создание журналов
description: Создает объект журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3c90808de4f07e45ded7c215577fff6916a59978
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431433"
---
# <a name="create-journals"></a><span data-ttu-id="c397d-103">Создание журналов</span><span class="sxs-lookup"><span data-stu-id="c397d-103">Create journals</span></span>

<span data-ttu-id="c397d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c397d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c397d-105">Создает журнал в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="c397d-105">Creates a journal in Dynamics 365 Business Central.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c397d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c397d-106">Permissions</span></span>
<span data-ttu-id="c397d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c397d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c397d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c397d-109">Permission type</span></span> |<span data-ttu-id="c397d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c397d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c397d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c397d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c397d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c397d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c397d-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c397d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c397d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c397d-114">Not supported.</span></span>|
|<span data-ttu-id="c397d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c397d-115">Application</span></span>|<span data-ttu-id="c397d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c397d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c397d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c397d-117">HTTP request</span></span>

```
POST /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c397d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c397d-118">Optional query parameters</span></span>
<span data-ttu-id="c397d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c397d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c397d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c397d-120">Request headers</span></span>
|<span data-ttu-id="c397d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c397d-121">Header</span></span>        |<span data-ttu-id="c397d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c397d-122">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="c397d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c397d-123">Authorization</span></span> |<span data-ttu-id="c397d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c397d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c397d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c397d-126">Content-Type</span></span>  |<span data-ttu-id="c397d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c397d-127">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="c397d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c397d-128">Request body</span></span>
<span data-ttu-id="c397d-129">В тексте запроса добавьте представление объекта **журналов** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c397d-129">In the request body, supply a JSON representation of a **journals** object.</span></span>

## <a name="response"></a><span data-ttu-id="c397d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c397d-130">Response</span></span>
<span data-ttu-id="c397d-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **журналов** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c397d-131">If successful, this method returns ```201 Created``` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c397d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c397d-132">Example</span></span>

<span data-ttu-id="c397d-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="c397d-133">**Request**</span></span>

<span data-ttu-id="c397d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c397d-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/journals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="c397d-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="c397d-135">**Response**</span></span>

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

