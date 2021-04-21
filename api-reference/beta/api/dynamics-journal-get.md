---
title: Получать журналы
description: Получает объект журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e814dd9afe56633c15825ede842f799bd85b0700
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921674"
---
# <a name="get-journals"></a><span data-ttu-id="6d58b-103">Получать журналы</span><span class="sxs-lookup"><span data-stu-id="6d58b-103">Get journals</span></span>

<span data-ttu-id="6d58b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d58b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d58b-105">Извлечение свойств и связей объекта журнала для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="6d58b-105">Retrieve the properties and relationships of a journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d58b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d58b-106">Permissions</span></span>
<span data-ttu-id="6d58b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d58b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d58b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d58b-109">Permission type</span></span> |<span data-ttu-id="6d58b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d58b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6d58b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d58b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d58b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d58b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6d58b-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d58b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6d58b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d58b-114">Not supported.</span></span>|
|<span data-ttu-id="6d58b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6d58b-115">Application</span></span>|<span data-ttu-id="6d58b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d58b-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d58b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d58b-117">HTTP request</span></span>

```http
GET /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d58b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6d58b-118">Optional query parameters</span></span>
<span data-ttu-id="6d58b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6d58b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d58b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d58b-120">Request headers</span></span>
|<span data-ttu-id="6d58b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d58b-121">Header</span></span>|<span data-ttu-id="6d58b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d58b-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="6d58b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d58b-123">Authorization</span></span>  |<span data-ttu-id="6d58b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d58b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d58b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d58b-126">Request body</span></span>
<span data-ttu-id="6d58b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d58b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d58b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d58b-128">Response</span></span>
<span data-ttu-id="6d58b-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` **журналов** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6d58b-129">If successful, this method returns a `200 OK` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d58b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6d58b-130">Example</span></span>

<span data-ttu-id="6d58b-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="6d58b-131">**Request**</span></span>

<span data-ttu-id="6d58b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d58b-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}
```

<span data-ttu-id="6d58b-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="6d58b-133">**Response**</span></span>

<span data-ttu-id="6d58b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6d58b-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="6d58b-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6d58b-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d58b-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d58b-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



