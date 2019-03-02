---
title: Удаление Каунтриесрегионс
description: Удаляет объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6897e072ca18be4f87405ca063f92df8d2f2a50b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365341"
---
# <a name="delete-countriesregions"></a><span data-ttu-id="16bf6-103">Удаление Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="16bf6-103">Delete countriesRegions</span></span>
<span data-ttu-id="16bf6-104">Удаление объекта стран и регионов из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="16bf6-104">Delete a countries/regions object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="16bf6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16bf6-105">Permissions</span></span>
<span data-ttu-id="16bf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16bf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16bf6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16bf6-108">Permission type</span></span> |<span data-ttu-id="16bf6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16bf6-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="16bf6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16bf6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="16bf6-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16bf6-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="16bf6-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16bf6-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="16bf6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16bf6-113">Not supported.</span></span>|
|<span data-ttu-id="16bf6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16bf6-114">Application</span></span>|<span data-ttu-id="16bf6-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16bf6-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16bf6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16bf6-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/countriesRegions('{id}')
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16bf6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16bf6-117">Optional query parameters</span></span>
<span data-ttu-id="16bf6-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16bf6-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16bf6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16bf6-119">Request headers</span></span>
|<span data-ttu-id="16bf6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16bf6-120">Header</span></span>|<span data-ttu-id="16bf6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16bf6-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="16bf6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16bf6-122">Authorization</span></span>  |<span data-ttu-id="16bf6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16bf6-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="16bf6-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="16bf6-125">If-Match</span></span>       |<span data-ttu-id="16bf6-126">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="16bf6-126">Required.</span></span> <span data-ttu-id="16bf6-127">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **каунтриесрегионс**, **каунтриесрегионс** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="16bf6-127">When this request header is included and the eTag provided does not match the current tag on the **countriesRegions**, the **countriesRegions** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16bf6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16bf6-128">Request body</span></span>
<span data-ttu-id="16bf6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16bf6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16bf6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="16bf6-130">Response</span></span>
<span data-ttu-id="16bf6-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="16bf6-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16bf6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="16bf6-133">Example</span></span>

<span data-ttu-id="16bf6-134">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="16bf6-134">**Request**</span></span>

<span data-ttu-id="16bf6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16bf6-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/countriesRegions('{id}')
```

<span data-ttu-id="16bf6-136">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="16bf6-136">**Response**</span></span> 

<span data-ttu-id="16bf6-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16bf6-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
