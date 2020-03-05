---
title: Удаление Таксареас
description: Удаляет объект налоговой области в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: d5e5f83b1d7cc900e8ac791af18c3e5c28b321eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42428336"
---
# <a name="delete-taxareas"></a><span data-ttu-id="f0eeb-103">Удаление Таксареас</span><span class="sxs-lookup"><span data-stu-id="f0eeb-103">Delete taxAreas</span></span>

<span data-ttu-id="f0eeb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f0eeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0eeb-105">Удаление объекта налоговой области из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-105">Delete a tax area object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0eeb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0eeb-106">Permissions</span></span>
<span data-ttu-id="f0eeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0eeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0eeb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0eeb-109">Permission type</span></span> |<span data-ttu-id="f0eeb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0eeb-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f0eeb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0eeb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0eeb-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0eeb-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f0eeb-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0eeb-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f0eeb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-114">Not supported.</span></span>|
|<span data-ttu-id="f0eeb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0eeb-115">Application</span></span>|<span data-ttu-id="f0eeb-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0eeb-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0eeb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0eeb-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0eeb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0eeb-118">Optional query parameters</span></span>
<span data-ttu-id="f0eeb-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0eeb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0eeb-120">Request headers</span></span>
|<span data-ttu-id="f0eeb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0eeb-121">Header</span></span>|<span data-ttu-id="f0eeb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0eeb-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="f0eeb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0eeb-123">Authorization</span></span>  |<span data-ttu-id="f0eeb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f0eeb-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="f0eeb-126">If-Match</span></span>       |<span data-ttu-id="f0eeb-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-127">Required.</span></span> <span data-ttu-id="f0eeb-128">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **таксареас**, **таксареас** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-128">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0eeb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0eeb-129">Request body</span></span>

<span data-ttu-id="f0eeb-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0eeb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0eeb-131">Response</span></span>

<span data-ttu-id="f0eeb-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0eeb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f0eeb-134">Example</span></span>

<span data-ttu-id="f0eeb-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="f0eeb-135">**Request**</span></span>

<span data-ttu-id="f0eeb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
```

<span data-ttu-id="f0eeb-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="f0eeb-137">**Response**</span></span> 

<span data-ttu-id="f0eeb-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0eeb-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
