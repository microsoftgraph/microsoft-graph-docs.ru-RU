---
title: Создание Пайментмесодс
description: Создает объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 08ef2450c06040820dac0b1807c16382bff262dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458623"
---
# <a name="create-paymentmethods"></a><span data-ttu-id="816d4-103">Создание Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="816d4-103">Create paymentMethods</span></span>
<span data-ttu-id="816d4-104">Создайте объект метода оплаты в Ддинамикс 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="816d4-104">Create a payment method object in DDynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="816d4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="816d4-105">Permissions</span></span>
<span data-ttu-id="816d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="816d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="816d4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="816d4-108">Permission type</span></span> |<span data-ttu-id="816d4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="816d4-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="816d4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="816d4-110">Delegated (work or school account)</span></span>|<span data-ttu-id="816d4-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="816d4-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="816d4-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="816d4-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="816d4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="816d4-113">Not supported.</span></span>|
|<span data-ttu-id="816d4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="816d4-114">Application</span></span>|<span data-ttu-id="816d4-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="816d4-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="816d4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="816d4-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/paymentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="816d4-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="816d4-117">Optional query parameters</span></span>
<span data-ttu-id="816d4-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="816d4-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="816d4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="816d4-119">Request headers</span></span>
|<span data-ttu-id="816d4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="816d4-120">Header</span></span>         |<span data-ttu-id="816d4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="816d4-121">Value</span></span>                        |
|---------------|-----------------------------|
|<span data-ttu-id="816d4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="816d4-122">Authorization</span></span>  |<span data-ttu-id="816d4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="816d4-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="816d4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="816d4-125">Content-Type</span></span>   |<span data-ttu-id="816d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="816d4-126">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="816d4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="816d4-127">Request body</span></span>
<span data-ttu-id="816d4-128">В тексте запроса добавьте представление объекта **Пайментмесодс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="816d4-128">In the request body, supply a JSON representation of a **paymentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="816d4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="816d4-129">Response</span></span>
<span data-ttu-id="816d4-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **пайментмесодс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="816d4-130">If successful, this method returns ```201 Created``` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="816d4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="816d4-131">Example</span></span>

<span data-ttu-id="816d4-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="816d4-132">**Request**</span></span>

<span data-ttu-id="816d4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="816d4-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
}
```

<span data-ttu-id="816d4-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="816d4-134">**Response**</span></span>

<span data-ttu-id="816d4-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="816d4-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="816d4-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="816d4-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="816d4-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="816d4-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}

```

