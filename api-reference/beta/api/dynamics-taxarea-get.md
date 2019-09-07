---
title: Получение Таксареас
description: Получает объект налоговой области в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 50c119a08e547d87afa2eeb40e790b5e98e7b68d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791255"
---
# <a name="get-taxareas"></a><span data-ttu-id="fa8a2-103">Получение Таксареас</span><span class="sxs-lookup"><span data-stu-id="fa8a2-103">Get taxAreas</span></span>
<span data-ttu-id="fa8a2-104">Получение свойств и связей объекта налоговой области для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-104">Retrieve the properties and relationships of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa8a2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa8a2-105">Permissions</span></span>
<span data-ttu-id="fa8a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa8a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa8a2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa8a2-108">Permission type</span></span> |<span data-ttu-id="fa8a2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa8a2-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="fa8a2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa8a2-110">Delegated (work or school account)</span></span>|<span data-ttu-id="fa8a2-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa8a2-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="fa8a2-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa8a2-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fa8a2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-113">Not supported.</span></span>|
|<span data-ttu-id="fa8a2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa8a2-114">Application</span></span>|<span data-ttu-id="fa8a2-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa8a2-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa8a2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa8a2-116">HTTP request</span></span>

```
GET /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa8a2-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa8a2-117">Optional query parameters</span></span>
<span data-ttu-id="fa8a2-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa8a2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa8a2-119">Request headers</span></span>
|<span data-ttu-id="fa8a2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa8a2-120">Header</span></span>|<span data-ttu-id="fa8a2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fa8a2-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="fa8a2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa8a2-122">Authorization</span></span>  |<span data-ttu-id="fa8a2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa8a2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa8a2-125">Request body</span></span>
<span data-ttu-id="fa8a2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa8a2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa8a2-127">Response</span></span>
<span data-ttu-id="fa8a2-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **таксареас** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-128">If successful, this method returns a `200 OK` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa8a2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fa8a2-129">Example</span></span>

<span data-ttu-id="fa8a2-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="fa8a2-130">**Request**</span></span>

<span data-ttu-id="fa8a2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
```

<span data-ttu-id="fa8a2-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="fa8a2-132">**Response**</span></span>

<span data-ttu-id="fa8a2-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="fa8a2-134">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fa8a2-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa8a2-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

