---
title: Удаление Итемкатегориес
description: Удаляет категорию элементов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 0b0d848af5389e26b53effb70063ee07ae5d4714
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956221"
---
# <a name="delete-itemcategories"></a><span data-ttu-id="87174-103">Удаление Итемкатегориес</span><span class="sxs-lookup"><span data-stu-id="87174-103">Delete itemCategories</span></span>
<span data-ttu-id="87174-104">Удаление Итемкатегори из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="87174-104">Delete an itemCategory from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="87174-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87174-105">Permissions</span></span>
<span data-ttu-id="87174-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87174-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87174-108">Permission type</span></span> |<span data-ttu-id="87174-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87174-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="87174-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87174-110">Delegated (work or school account)</span></span>|<span data-ttu-id="87174-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87174-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="87174-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87174-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="87174-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87174-113">Not supported.</span></span>|
|<span data-ttu-id="87174-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87174-114">Application</span></span>|<span data-ttu-id="87174-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87174-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87174-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87174-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/itemCategories('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87174-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="87174-117">Optional query parameters</span></span>
<span data-ttu-id="87174-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="87174-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87174-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87174-119">Request headers</span></span>
|<span data-ttu-id="87174-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87174-120">Header</span></span>         |<span data-ttu-id="87174-121">Значение</span><span class="sxs-lookup"><span data-stu-id="87174-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="87174-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87174-122">Authorization</span></span>  |<span data-ttu-id="87174-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87174-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="87174-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="87174-125">If-Match</span></span>       |<span data-ttu-id="87174-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="87174-126">Required.</span></span> <span data-ttu-id="87174-127">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **итемкатегориес**, **итемкатегориес** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="87174-127">When this request header is included and the eTag provided does not match the current tag on the **itemCategories**, the **itemCategories** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87174-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87174-128">Request body</span></span>
<span data-ttu-id="87174-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87174-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87174-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="87174-130">Response</span></span>
<span data-ttu-id="87174-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="87174-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87174-133">Пример</span><span class="sxs-lookup"><span data-stu-id="87174-133">Example</span></span>

<span data-ttu-id="87174-134">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="87174-134">**Request**</span></span>

<span data-ttu-id="87174-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87174-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/itemCategories('{id}')
```

<span data-ttu-id="87174-136">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="87174-136">**Response**</span></span> 

<span data-ttu-id="87174-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="87174-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```

