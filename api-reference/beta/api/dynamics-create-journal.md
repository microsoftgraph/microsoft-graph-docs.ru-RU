---
title: Создание журналов
description: Создает объект журнала в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e67c1692ce6a0e6579070f0c8d420798e67c4e61
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473289"
---
# <a name="create-journals"></a><span data-ttu-id="a5273-103">Создание журналов</span><span class="sxs-lookup"><span data-stu-id="a5273-103">Create journals</span></span>

<span data-ttu-id="a5273-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5273-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5273-105">Создает журнал в Центре бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a5273-105">Creates a journal in Dynamics 365 Business Central.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a5273-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5273-106">Permissions</span></span>
<span data-ttu-id="a5273-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5273-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5273-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5273-109">Permission type</span></span> |<span data-ttu-id="a5273-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5273-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a5273-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5273-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5273-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5273-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a5273-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5273-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a5273-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5273-114">Not supported.</span></span>|
|<span data-ttu-id="a5273-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5273-115">Application</span></span>|<span data-ttu-id="a5273-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5273-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5273-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5273-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5273-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5273-118">Optional query parameters</span></span>
<span data-ttu-id="a5273-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a5273-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5273-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5273-120">Request headers</span></span>
|<span data-ttu-id="a5273-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5273-121">Header</span></span>        |<span data-ttu-id="a5273-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5273-122">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="a5273-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5273-123">Authorization</span></span> |<span data-ttu-id="a5273-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5273-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="a5273-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5273-126">Content-Type</span></span>  |<span data-ttu-id="a5273-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a5273-127">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="a5273-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5273-128">Request body</span></span>
<span data-ttu-id="a5273-129">В теле запроса поставляем представление JSON объекта **журналов.**</span><span class="sxs-lookup"><span data-stu-id="a5273-129">In the request body, supply a JSON representation of a **journals** object.</span></span>

## <a name="response"></a><span data-ttu-id="a5273-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5273-130">Response</span></span>
<span data-ttu-id="a5273-131">В случае успешной работы этот метод возвращает код ответа и объект ```201 Created``` **журналов** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5273-131">If successful, this method returns ```201 Created``` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5273-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a5273-132">Example</span></span>

<span data-ttu-id="a5273-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="a5273-133">**Request**</span></span>

<span data-ttu-id="a5273-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5273-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/journals
Content-type: application/json

{
  "code": "DEFAULT"
}
```

<span data-ttu-id="a5273-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="a5273-135">**Response**</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



