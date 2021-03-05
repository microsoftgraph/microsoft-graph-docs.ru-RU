---
title: Создание taxAreas
description: Создает объект налоговой области в Dynamics for Financials.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e30275efd4205b776593b5d515b2032654506a90
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473247"
---
# <a name="create-taxareas"></a><span data-ttu-id="848a5-103">Создание taxAreas</span><span class="sxs-lookup"><span data-stu-id="848a5-103">Create taxAreas</span></span>

<span data-ttu-id="848a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="848a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="848a5-105">Создает объект области налогообложения в Центре бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="848a5-105">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="848a5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="848a5-106">Permissions</span></span>
<span data-ttu-id="848a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="848a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="848a5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="848a5-109">Permission type</span></span> |<span data-ttu-id="848a5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="848a5-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="848a5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="848a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="848a5-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="848a5-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="848a5-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="848a5-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="848a5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="848a5-114">Not supported.</span></span>|
|<span data-ttu-id="848a5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="848a5-115">Application</span></span>|<span data-ttu-id="848a5-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="848a5-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="848a5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="848a5-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="848a5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="848a5-118">Optional query parameters</span></span>
<span data-ttu-id="848a5-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="848a5-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="848a5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="848a5-120">Request headers</span></span>
|<span data-ttu-id="848a5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="848a5-121">Header</span></span>|<span data-ttu-id="848a5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="848a5-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="848a5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="848a5-123">Authorization</span></span>  |<span data-ttu-id="848a5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="848a5-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="848a5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="848a5-126">Content-Type</span></span>  |<span data-ttu-id="848a5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="848a5-127">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="848a5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="848a5-128">Request body</span></span>
<span data-ttu-id="848a5-129">В теле запроса укажи представление JSON объекта **taxAreas.**</span><span class="sxs-lookup"><span data-stu-id="848a5-129">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="848a5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="848a5-130">Response</span></span>
<span data-ttu-id="848a5-131">В случае успешной работы этот метод возвращает код ответа и объект ```201 Created``` **taxAreas** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="848a5-131">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="848a5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="848a5-132">Example</span></span>

<span data-ttu-id="848a5-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="848a5-133">**Request**</span></span>

<span data-ttu-id="848a5-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="848a5-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas
Content-type: application/json

{
  "code": "44442001T"
}
```

<span data-ttu-id="848a5-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="848a5-135">**Response**</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "44442001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


