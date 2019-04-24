---
title: удалять элементы.
description: Удаляет объект item в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b8b03c12ccc4592af97ee4160ca317eac65f73f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458483"
---
# <a name="delete-items"></a><span data-ttu-id="41c97-103">удалять элементы.</span><span class="sxs-lookup"><span data-stu-id="41c97-103">Delete items</span></span>
<span data-ttu-id="41c97-104">Удаление элемента из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="41c97-104">Delete an item from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="41c97-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41c97-105">Permissions</span></span>
<span data-ttu-id="41c97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41c97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c97-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41c97-108">Permission type</span></span> |<span data-ttu-id="41c97-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41c97-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="41c97-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41c97-110">Delegated (work or school account)</span></span>|<span data-ttu-id="41c97-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41c97-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="41c97-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41c97-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="41c97-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41c97-113">Not supported.</span></span>|
|<span data-ttu-id="41c97-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41c97-114">Application</span></span>|<span data-ttu-id="41c97-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41c97-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41c97-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41c97-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/items('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41c97-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41c97-117">Optional query parameters</span></span>
<span data-ttu-id="41c97-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="41c97-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41c97-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41c97-119">Request headers</span></span>
|<span data-ttu-id="41c97-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41c97-120">Header</span></span>       |<span data-ttu-id="41c97-121">Значение</span><span class="sxs-lookup"><span data-stu-id="41c97-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="41c97-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41c97-122">Authorization</span></span>|<span data-ttu-id="41c97-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41c97-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="41c97-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="41c97-125">If-Match</span></span>     |<span data-ttu-id="41c97-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="41c97-126">Required.</span></span> <span data-ttu-id="41c97-127">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу **элементов**, **элементы** не будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="41c97-127">When this request header is included and the eTag provided does not match the current tag on the **items**, the **items** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41c97-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41c97-128">Request body</span></span>
<span data-ttu-id="41c97-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41c97-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41c97-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="41c97-130">Response</span></span>
<span data-ttu-id="41c97-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="41c97-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41c97-133">Пример</span><span class="sxs-lookup"><span data-stu-id="41c97-133">Example</span></span>

<span data-ttu-id="41c97-134">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="41c97-134">**Request**</span></span>

<span data-ttu-id="41c97-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41c97-135">Here is an example of the request.</span></span>
```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/items('{id}')
```

<span data-ttu-id="41c97-136">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="41c97-136">**Response**</span></span>

<span data-ttu-id="41c97-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="41c97-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```

