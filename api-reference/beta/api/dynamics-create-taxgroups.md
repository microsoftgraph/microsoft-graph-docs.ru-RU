---
title: Создание Таксграупс
description: Создает объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8bc45dfbb7efe2d2f5fcc3ab33af38331621445b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431150"
---
# <a name="create-taxgroups"></a><span data-ttu-id="ba712-103">Создание Таксграупс</span><span class="sxs-lookup"><span data-stu-id="ba712-103">Create taxGroups</span></span>

<span data-ttu-id="ba712-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ba712-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba712-105">Создайте объект налоговой группы в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="ba712-105">Create a tax groups object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba712-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba712-106">Permissions</span></span>
<span data-ttu-id="ba712-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba712-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba712-109">Permission type</span></span> |<span data-ttu-id="ba712-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba712-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ba712-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba712-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba712-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba712-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ba712-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba712-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ba712-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba712-114">Not supported.</span></span>|
|<span data-ttu-id="ba712-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba712-115">Application</span></span>|<span data-ttu-id="ba712-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba712-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba712-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba712-117">HTTP request</span></span>
```
POST /financials/companies/{id}/taxGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba712-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba712-118">Optional query parameters</span></span>
<span data-ttu-id="ba712-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ba712-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba712-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba712-120">Request headers</span></span>

|<span data-ttu-id="ba712-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba712-121">Header</span></span>|<span data-ttu-id="ba712-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ba712-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="ba712-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba712-123">Authorization</span></span>  |<span data-ttu-id="ba712-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba712-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="ba712-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba712-126">Content-Type</span></span>  |<span data-ttu-id="ba712-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ba712-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="ba712-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba712-128">Request body</span></span>
<span data-ttu-id="ba712-129">В тексте запроса добавьте представление объекта **таксграупс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba712-129">In the request body, supply a JSON representation of a **taxGroups** object.</span></span>

## <a name="response"></a><span data-ttu-id="ba712-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba712-130">Response</span></span>
<span data-ttu-id="ba712-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **таксграупс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba712-131">If successful, this method returns ```201 Created``` response code and a **taxGroups** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba712-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ba712-132">Example</span></span>

<span data-ttu-id="ba712-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="ba712-133">**Request**</span></span>

<span data-ttu-id="ba712-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba712-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxGroups
Content-type: application/json

{
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax"
}
```

<span data-ttu-id="ba712-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="ba712-135">**Response**</span></span>

<span data-ttu-id="ba712-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba712-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="ba712-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ba712-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ba712-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba712-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}

```
