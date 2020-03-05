---
title: Получение учетных записей
description: Возвращает объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ca6c8fdc7dd65bbbaab9f6829eb9395d80e950d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432147"
---
# <a name="get-accounts"></a><span data-ttu-id="ae190-103">Получение учетных записей</span><span class="sxs-lookup"><span data-stu-id="ae190-103">Get accounts</span></span>

<span data-ttu-id="ae190-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ae190-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae190-105">Получение свойств и связей объекта Account для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="ae190-105">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae190-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae190-106">Permissions</span></span>
<span data-ttu-id="ae190-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae190-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae190-109">Permission type</span></span> |<span data-ttu-id="ae190-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae190-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ae190-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae190-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ae190-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae190-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ae190-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae190-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ae190-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae190-114">Not supported.</span></span>|
|<span data-ttu-id="ae190-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae190-115">Application</span></span>|<span data-ttu-id="ae190-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae190-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="ae190-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae190-117">HTTP request</span></span>
```
GET /financials/companies/{id}/accounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae190-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae190-118">Optional query parameters</span></span>
<span data-ttu-id="ae190-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae190-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae190-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae190-120">Request headers</span></span>
|<span data-ttu-id="ae190-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae190-121">Header</span></span>|<span data-ttu-id="ae190-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ae190-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="ae190-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae190-123">Authorization</span></span>  |<span data-ttu-id="ae190-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae190-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae190-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae190-126">Request body</span></span>
<span data-ttu-id="ae190-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae190-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae190-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae190-128">Response</span></span>
<span data-ttu-id="ae190-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **Accounts** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae190-129">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae190-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ae190-130">Example</span></span>

<span data-ttu-id="ae190-131">**Request (запрос** ) Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae190-131">**Request** Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/accounts/{id}
```

<span data-ttu-id="ae190-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="ae190-132">**Response**</span></span>

<span data-ttu-id="ae190-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae190-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="ae190-134">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ae190-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ae190-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae190-135">All the properties will be returned from an actual call.</span></span>

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