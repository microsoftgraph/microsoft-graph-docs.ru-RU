---
title: Удаление поставщиков
description: Удаляет объект поставщика в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8de331472d60c64ac753243f3bbcba18d23b3a24
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474101"
---
# <a name="delete-vendors"></a><span data-ttu-id="9167b-103">Удаление поставщиков</span><span class="sxs-lookup"><span data-stu-id="9167b-103">Delete vendors</span></span>

<span data-ttu-id="9167b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9167b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9167b-105">Удаление объекта поставщика из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9167b-105">Delete a vendor object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9167b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9167b-106">Permissions</span></span>
<span data-ttu-id="9167b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9167b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9167b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9167b-109">Permission type</span></span> |<span data-ttu-id="9167b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9167b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9167b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9167b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9167b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9167b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9167b-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9167b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9167b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9167b-114">Not supported.</span></span>|
|<span data-ttu-id="9167b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9167b-115">Application</span></span>|<span data-ttu-id="9167b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9167b-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9167b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9167b-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/vendors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9167b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9167b-118">Optional query parameters</span></span>
<span data-ttu-id="9167b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9167b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9167b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9167b-120">Request headers</span></span>
|<span data-ttu-id="9167b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9167b-121">Header</span></span>|<span data-ttu-id="9167b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9167b-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="9167b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9167b-123">Authorization</span></span>  |<span data-ttu-id="9167b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9167b-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9167b-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="9167b-126">If-Match</span></span>       |<span data-ttu-id="9167b-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9167b-127">Required.</span></span> <span data-ttu-id="9167b-128">Если эта заглавная версия запроса включена и предоставленный eTag  не соответствует текущему тегу поставщиков, поставщики не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="9167b-128">When this request header is included and the eTag provided does not match the current tag on the **vendors**, the **vendors** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9167b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9167b-129">Request body</span></span>
<span data-ttu-id="9167b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9167b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9167b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9167b-131">Response</span></span>
<span data-ttu-id="9167b-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9167b-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9167b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="9167b-134">Example</span></span>

<span data-ttu-id="9167b-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="9167b-135">**Request**</span></span>

<span data-ttu-id="9167b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9167b-136">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/vendors/{id}
```

<span data-ttu-id="9167b-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="9167b-137">**Response**</span></span> 

<span data-ttu-id="9167b-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9167b-138">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```


