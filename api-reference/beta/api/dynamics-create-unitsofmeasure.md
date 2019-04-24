---
title: Создание Унитсофмеасуре
description: Создает объект единицы измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a0020ab72ee7bcbbe2b229f209d52bc68691dcb2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458574"
---
# <a name="create-unitsofmeasure"></a><span data-ttu-id="36c71-103">Создание Унитсофмеасуре</span><span class="sxs-lookup"><span data-stu-id="36c71-103">Create unitsOfMeasure</span></span>
<span data-ttu-id="36c71-104">Создайте объект единицы измерения в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="36c71-104">Create a units of measure object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="36c71-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36c71-105">Permissions</span></span>
<span data-ttu-id="36c71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36c71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c71-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36c71-108">Permission type</span></span> |<span data-ttu-id="36c71-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36c71-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="36c71-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36c71-110">Delegated (work or school account)</span></span>|<span data-ttu-id="36c71-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c71-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="36c71-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36c71-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="36c71-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36c71-113">Not supported.</span></span>|
|<span data-ttu-id="36c71-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36c71-114">Application</span></span>|<span data-ttu-id="36c71-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c71-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36c71-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36c71-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/unitsOfMeasure
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36c71-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="36c71-117">Optional query parameters</span></span>
<span data-ttu-id="36c71-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="36c71-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36c71-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36c71-119">Request headers</span></span>
|<span data-ttu-id="36c71-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36c71-120">Header</span></span>|<span data-ttu-id="36c71-121">Значение</span><span class="sxs-lookup"><span data-stu-id="36c71-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="36c71-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36c71-122">Authorization</span></span>  |<span data-ttu-id="36c71-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36c71-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="36c71-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36c71-125">Content-Type</span></span>  |<span data-ttu-id="36c71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36c71-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="36c71-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36c71-127">Request body</span></span>
<span data-ttu-id="36c71-128">В тексте запроса добавьте представление объекта **Унитсофмеасуре** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36c71-128">In the request body, supply a JSON representation of a **unitsOfMeasure** object.</span></span>

## <a name="response"></a><span data-ttu-id="36c71-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="36c71-129">Response</span></span>
<span data-ttu-id="36c71-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **унитсофмеасуре** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36c71-130">If successful, this method returns ```201 Created``` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36c71-131">Пример</span><span class="sxs-lookup"><span data-stu-id="36c71-131">Example</span></span>

<span data-ttu-id="36c71-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="36c71-132">**Request**</span></span>

<span data-ttu-id="36c71-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36c71-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/unitsOfMeasure
Content-type: application/json

{
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA"
}
```

<span data-ttu-id="36c71-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="36c71-134">**Response**</span></span>

<span data-ttu-id="36c71-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36c71-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="36c71-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36c71-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="36c71-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36c71-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}

```

