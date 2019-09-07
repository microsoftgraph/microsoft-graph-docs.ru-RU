---
title: Создание Таксареас
description: Создает объект налоговой области в Dynamics для финансовых показателей.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 9dc553ac9fbd0bbbbe45e7775ffd91f2f4cdb881
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791899"
---
# <a name="create-taxareas"></a><span data-ttu-id="a6b2e-103">Создание Таксареас</span><span class="sxs-lookup"><span data-stu-id="a6b2e-103">Create taxAreas</span></span>
<span data-ttu-id="a6b2e-104">Создает объект налоговой области в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a6b2e-104">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6b2e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6b2e-105">Permissions</span></span>
<span data-ttu-id="a6b2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6b2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6b2e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6b2e-108">Permission type</span></span> |<span data-ttu-id="a6b2e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6b2e-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a6b2e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6b2e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="a6b2e-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b2e-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a6b2e-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6b2e-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a6b2e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6b2e-113">Not supported.</span></span>|
|<span data-ttu-id="a6b2e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6b2e-114">Application</span></span>|<span data-ttu-id="a6b2e-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b2e-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6b2e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6b2e-116">HTTP request</span></span>

```
POST /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6b2e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6b2e-117">Optional query parameters</span></span>
<span data-ttu-id="a6b2e-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6b2e-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6b2e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6b2e-119">Request headers</span></span>
|<span data-ttu-id="a6b2e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6b2e-120">Header</span></span>|<span data-ttu-id="a6b2e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a6b2e-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="a6b2e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6b2e-122">Authorization</span></span>  |<span data-ttu-id="a6b2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6b2e-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="a6b2e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6b2e-125">Content-Type</span></span>  |<span data-ttu-id="a6b2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6b2e-126">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="a6b2e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6b2e-127">Request body</span></span>
<span data-ttu-id="a6b2e-128">В тексте запроса добавьте представление объекта **таксареас** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6b2e-128">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="a6b2e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6b2e-129">Response</span></span>
<span data-ttu-id="a6b2e-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **таксареас** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6b2e-130">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6b2e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a6b2e-131">Example</span></span>

<span data-ttu-id="a6b2e-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="a6b2e-132">**Request**</span></span>

<span data-ttu-id="a6b2e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6b2e-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas
Content-type: application/json

```json
{
  "code": "44442001T"
}
```

<span data-ttu-id="a6b2e-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="a6b2e-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "44442001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```
