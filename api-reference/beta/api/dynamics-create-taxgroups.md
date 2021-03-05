---
title: Создание taxGroups
description: Создает объект группы налогообложения в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 30fc1054dc3a9851c8dc18ffb7de05224d08285c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473222"
---
# <a name="create-taxgroups"></a><span data-ttu-id="a13fa-103">Создание taxGroups</span><span class="sxs-lookup"><span data-stu-id="a13fa-103">Create taxGroups</span></span>

<span data-ttu-id="a13fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a13fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a13fa-105">Создание объекта налоговых групп в Центре бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a13fa-105">Create a tax groups object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a13fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a13fa-106">Permissions</span></span>
<span data-ttu-id="a13fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a13fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a13fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a13fa-109">Permission type</span></span> |<span data-ttu-id="a13fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a13fa-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a13fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a13fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a13fa-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a13fa-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a13fa-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a13fa-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a13fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a13fa-114">Not supported.</span></span>|
|<span data-ttu-id="a13fa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a13fa-115">Application</span></span>|<span data-ttu-id="a13fa-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a13fa-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a13fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a13fa-117">HTTP request</span></span>
```
POST /financials/companies/{id}/taxGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a13fa-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a13fa-118">Optional query parameters</span></span>
<span data-ttu-id="a13fa-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a13fa-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a13fa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a13fa-120">Request headers</span></span>

|<span data-ttu-id="a13fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a13fa-121">Header</span></span>|<span data-ttu-id="a13fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a13fa-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="a13fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a13fa-123">Authorization</span></span>  |<span data-ttu-id="a13fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a13fa-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="a13fa-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a13fa-126">Content-Type</span></span>  |<span data-ttu-id="a13fa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a13fa-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="a13fa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a13fa-128">Request body</span></span>
<span data-ttu-id="a13fa-129">В органе запроса поставляем представление JSON объекта **taxGroups.**</span><span class="sxs-lookup"><span data-stu-id="a13fa-129">In the request body, supply a JSON representation of a **taxGroups** object.</span></span>

## <a name="response"></a><span data-ttu-id="a13fa-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a13fa-130">Response</span></span>
<span data-ttu-id="a13fa-131">В случае успеха этот метод возвращает код ответа и ```201 Created``` **объект taxGroups** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a13fa-131">If successful, this method returns ```201 Created``` response code and a **taxGroups** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a13fa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a13fa-132">Example</span></span>

<span data-ttu-id="a13fa-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="a13fa-133">**Request**</span></span>

<span data-ttu-id="a13fa-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a13fa-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxGroups
Content-type: application/json

{
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax"
}
```

<span data-ttu-id="a13fa-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="a13fa-135">**Response**</span></span>

<span data-ttu-id="a13fa-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a13fa-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="a13fa-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a13fa-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a13fa-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a13fa-138">All the properties will be returned from an actual call.</span></span>

```http
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


