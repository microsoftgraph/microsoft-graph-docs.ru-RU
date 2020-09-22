---
title: Удаление Таксареас
description: Удаляет объект налоговой области в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3d50ae7f8e07a9338ba666e985d764e53a1f84c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008171"
---
# <a name="delete-taxareas"></a><span data-ttu-id="61c6c-103">Удаление Таксареас</span><span class="sxs-lookup"><span data-stu-id="61c6c-103">Delete taxAreas</span></span>

<span data-ttu-id="61c6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61c6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61c6c-105">Удаление объекта налоговой области из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="61c6c-105">Delete a tax area object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="61c6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61c6c-106">Permissions</span></span>
<span data-ttu-id="61c6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61c6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61c6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61c6c-109">Permission type</span></span> |<span data-ttu-id="61c6c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61c6c-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="61c6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61c6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61c6c-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61c6c-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="61c6c-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61c6c-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="61c6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61c6c-114">Not supported.</span></span>|
|<span data-ttu-id="61c6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61c6c-115">Application</span></span>|<span data-ttu-id="61c6c-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61c6c-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61c6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61c6c-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61c6c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="61c6c-118">Optional query parameters</span></span>
<span data-ttu-id="61c6c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="61c6c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61c6c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61c6c-120">Request headers</span></span>
|<span data-ttu-id="61c6c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61c6c-121">Header</span></span>|<span data-ttu-id="61c6c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="61c6c-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="61c6c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61c6c-123">Authorization</span></span>  |<span data-ttu-id="61c6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61c6c-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="61c6c-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="61c6c-126">If-Match</span></span>       |<span data-ttu-id="61c6c-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="61c6c-127">Required.</span></span> <span data-ttu-id="61c6c-128">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **таксареас**, **таксареас** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="61c6c-128">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61c6c-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61c6c-129">Request body</span></span>

<span data-ttu-id="61c6c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61c6c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61c6c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="61c6c-131">Response</span></span>

<span data-ttu-id="61c6c-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="61c6c-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61c6c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="61c6c-134">Example</span></span>

<span data-ttu-id="61c6c-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="61c6c-135">**Request**</span></span>

<span data-ttu-id="61c6c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61c6c-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
```

<span data-ttu-id="61c6c-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="61c6c-137">**Response**</span></span> 

<span data-ttu-id="61c6c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="61c6c-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```


