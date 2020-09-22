---
title: Создание журналов
description: Создает объект журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 529c56634579167d5cab3abd6a27634678087d75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981666"
---
# <a name="create-journals"></a><span data-ttu-id="5c483-103">Создание журналов</span><span class="sxs-lookup"><span data-stu-id="5c483-103">Create journals</span></span>

<span data-ttu-id="5c483-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c483-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c483-105">Создает журнал в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="5c483-105">Creates a journal in Dynamics 365 Business Central.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5c483-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c483-106">Permissions</span></span>
<span data-ttu-id="5c483-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c483-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c483-109">Permission type</span></span> |<span data-ttu-id="5c483-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c483-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5c483-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c483-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c483-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c483-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5c483-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c483-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5c483-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c483-114">Not supported.</span></span>|
|<span data-ttu-id="5c483-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c483-115">Application</span></span>|<span data-ttu-id="5c483-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c483-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c483-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c483-117">HTTP request</span></span>

```
POST /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c483-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c483-118">Optional query parameters</span></span>
<span data-ttu-id="5c483-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c483-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c483-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c483-120">Request headers</span></span>
|<span data-ttu-id="5c483-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c483-121">Header</span></span>        |<span data-ttu-id="5c483-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5c483-122">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="5c483-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c483-123">Authorization</span></span> |<span data-ttu-id="5c483-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c483-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="5c483-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c483-126">Content-Type</span></span>  |<span data-ttu-id="5c483-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5c483-127">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="5c483-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c483-128">Request body</span></span>
<span data-ttu-id="5c483-129">В тексте запроса добавьте представление объекта **журналов** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c483-129">In the request body, supply a JSON representation of a **journals** object.</span></span>

## <a name="response"></a><span data-ttu-id="5c483-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c483-130">Response</span></span>
<span data-ttu-id="5c483-131">В случае успешного выполнения этот метод возвращает ```201 Created``` код отклика и объект **журналов** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c483-131">If successful, this method returns ```201 Created``` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c483-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5c483-132">Example</span></span>

<span data-ttu-id="5c483-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5c483-133">**Request**</span></span>

<span data-ttu-id="5c483-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c483-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/journals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="5c483-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5c483-135">**Response**</span></span>

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



