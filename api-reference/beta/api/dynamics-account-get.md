---
title: Получить учетные записи
description: Получает объект учетной записи в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 0f3db2e969369198f716dbcde4c7147717fd47b1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046232"
---
# <a name="get-accounts"></a><span data-ttu-id="84506-103">Получить учетные записи</span><span class="sxs-lookup"><span data-stu-id="84506-103">Get accounts</span></span>

<span data-ttu-id="84506-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84506-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84506-105">Извлечение свойств и связей объекта учетной записи для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="84506-105">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="84506-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84506-106">Permissions</span></span>
<span data-ttu-id="84506-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84506-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84506-109">Permission type</span></span> |<span data-ttu-id="84506-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84506-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="84506-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84506-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84506-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84506-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="84506-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84506-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="84506-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84506-114">Not supported.</span></span>|
|<span data-ttu-id="84506-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84506-115">Application</span></span>|<span data-ttu-id="84506-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84506-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="84506-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84506-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/accounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84506-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84506-118">Optional query parameters</span></span>
<span data-ttu-id="84506-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84506-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84506-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84506-120">Request headers</span></span>
|<span data-ttu-id="84506-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84506-121">Header</span></span>|<span data-ttu-id="84506-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84506-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="84506-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84506-123">Authorization</span></span>  |<span data-ttu-id="84506-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84506-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84506-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84506-126">Request body</span></span>
<span data-ttu-id="84506-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84506-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84506-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="84506-128">Response</span></span>
<span data-ttu-id="84506-129">В случае успешной работы этот метод возвращает код ответа и объект учетных `200 OK` записей в  тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="84506-129">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84506-130">Пример</span><span class="sxs-lookup"><span data-stu-id="84506-130">Example</span></span>

<span data-ttu-id="84506-131">**Запрос** Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84506-131">**Request** Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/accounts/{id}
```

<span data-ttu-id="84506-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="84506-132">**Response**</span></span>

<span data-ttu-id="84506-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84506-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="84506-134">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="84506-134">**Note**: The response object shown here might be shortened for readability.</span></span>

```json
{
    "id": "id-value",
    "number": "10700",
    "displayName": "Inventory",
    "category": "Assets",
    "subCategory": "Inventory",
    "blocked": false,
    "lastModifiedDateTime": "2017-03-15T02:20:58.747Z"
}
```


