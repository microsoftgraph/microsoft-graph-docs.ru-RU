---
title: Получение учетных записей
description: Возвращает объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b020d6204a5c99f9b3a49721a3fc327f3314f4f7
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792235"
---
# <a name="get-accounts"></a><span data-ttu-id="3de28-103">Получение учетных записей</span><span class="sxs-lookup"><span data-stu-id="3de28-103">Get accounts</span></span>
<span data-ttu-id="3de28-104">Получение свойств и связей объекта Account для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="3de28-104">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3de28-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3de28-105">Permissions</span></span>
<span data-ttu-id="3de28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3de28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de28-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3de28-108">Permission type</span></span> |<span data-ttu-id="3de28-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3de28-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3de28-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3de28-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3de28-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de28-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3de28-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3de28-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3de28-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de28-113">Not supported.</span></span>|
|<span data-ttu-id="3de28-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3de28-114">Application</span></span>|<span data-ttu-id="3de28-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de28-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="3de28-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3de28-116">HTTP request</span></span>
```
GET /financials/companies/{id}/accounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3de28-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3de28-117">Optional query parameters</span></span>
<span data-ttu-id="3de28-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3de28-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3de28-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3de28-119">Request headers</span></span>
|<span data-ttu-id="3de28-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3de28-120">Header</span></span>|<span data-ttu-id="3de28-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3de28-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="3de28-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3de28-122">Authorization</span></span>  |<span data-ttu-id="3de28-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3de28-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3de28-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3de28-125">Request body</span></span>
<span data-ttu-id="3de28-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3de28-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3de28-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de28-127">Response</span></span>
<span data-ttu-id="3de28-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **Accounts** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3de28-128">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de28-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3de28-129">Example</span></span>

<span data-ttu-id="3de28-130">**Request (запрос** ) Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3de28-130">**Request** Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/accounts/{id}
```

<span data-ttu-id="3de28-131">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="3de28-131">**Response**</span></span>

<span data-ttu-id="3de28-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3de28-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="3de28-133">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3de28-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3de28-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3de28-134">All the properties will be returned from an actual call.</span></span>

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