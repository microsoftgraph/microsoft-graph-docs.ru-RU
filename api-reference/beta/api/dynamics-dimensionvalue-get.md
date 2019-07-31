---
title: Получение Дименсионвалуес
description: Возвращает объект значения измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c9b51a4291adfc6e446c428989aaa04b7540453d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956333"
---
# <a name="get-dimensionvalues"></a><span data-ttu-id="ea7bf-103">Получение Дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="ea7bf-103">Get dimensionValues</span></span>
<span data-ttu-id="ea7bf-104">Получение свойств и связей объекта значения измерения для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-104">Retrieve the properties and relationships of a dimension value object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea7bf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea7bf-105">Permissions</span></span>
<span data-ttu-id="ea7bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea7bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea7bf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea7bf-108">Permission type</span></span> |<span data-ttu-id="ea7bf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea7bf-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ea7bf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea7bf-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ea7bf-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea7bf-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ea7bf-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea7bf-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ea7bf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-113">Not supported.</span></span>|
|<span data-ttu-id="ea7bf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea7bf-114">Application</span></span>|<span data-ttu-id="ea7bf-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea7bf-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea7bf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea7bf-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/dimensions('{id}')/dimensionValues('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea7bf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea7bf-117">Optional query parameters</span></span>
<span data-ttu-id="ea7bf-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea7bf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea7bf-119">Request headers</span></span>
|<span data-ttu-id="ea7bf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea7bf-120">Header</span></span>       |<span data-ttu-id="ea7bf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ea7bf-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="ea7bf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea7bf-122">Authorization</span></span>|<span data-ttu-id="ea7bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea7bf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea7bf-125">Request body</span></span>
<span data-ttu-id="ea7bf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea7bf-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea7bf-127">Response</span></span>
<span data-ttu-id="ea7bf-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **дименсионвалуес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-128">If successful, this method returns a `200 OK` response code and a **dimensionValues** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea7bf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ea7bf-129">Example</span></span>

<span data-ttu-id="ea7bf-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="ea7bf-130">**Request**</span></span>

<span data-ttu-id="ea7bf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/dimensions('{id}')/dimensionValues('{id}')
```

<span data-ttu-id="ea7bf-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="ea7bf-132">**Response**</span></span>

<span data-ttu-id="ea7bf-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="ea7bf-134">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ea7bf-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea7bf-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "30",
  "displayName": "Europe North (EU)",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

