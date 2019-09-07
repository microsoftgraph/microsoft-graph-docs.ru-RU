---
title: Получение Ажедаккаунтспайабле
description: Возвращает устаревший объект кредиторской задолженности в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4884e6ba6d593160f3482de60bee3d358eb3a9ac
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792228"
---
# <a name="get-agedaccountspayable"></a><span data-ttu-id="f164b-103">Получение Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="f164b-103">Get agedAccountsPayable</span></span>
<span data-ttu-id="f164b-104">Получение свойств и связей для устаревших отчетов об оплате учетных записей для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f164b-104">Retrieve the properties and relationships of an aged accounts payable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f164b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f164b-105">Permissions</span></span>
<span data-ttu-id="f164b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f164b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f164b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f164b-108">Permission type</span></span> |<span data-ttu-id="f164b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f164b-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f164b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f164b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f164b-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f164b-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f164b-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f164b-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f164b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f164b-113">Not supported.</span></span>|
|<span data-ttu-id="f164b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f164b-114">Application</span></span>|<span data-ttu-id="f164b-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f164b-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f164b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f164b-116">HTTP request</span></span>
```
GET /financials/companies/{id}/agedAccountsPayable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f164b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f164b-117">Optional query parameters</span></span>
<span data-ttu-id="f164b-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f164b-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f164b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f164b-119">Request headers</span></span>
|<span data-ttu-id="f164b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f164b-120">Header</span></span>        |<span data-ttu-id="f164b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f164b-121">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="f164b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f164b-122">Authorization</span></span> |<span data-ttu-id="f164b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f164b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f164b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f164b-125">Request body</span></span>
<span data-ttu-id="f164b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f164b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f164b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f164b-127">Response</span></span>
<span data-ttu-id="f164b-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **ажедаккаунтспайабле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f164b-128">If successful, this method returns a `200 OK` response code and an **agedAccountsPayable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f164b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f164b-129">Example</span></span>

<span data-ttu-id="f164b-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="f164b-130">**Request**</span></span>

<span data-ttu-id="f164b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f164b-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/agedAccountsPayable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="f164b-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="f164b-132">**Response**</span></span>

<span data-ttu-id="f164b-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f164b-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="f164b-134">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f164b-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f164b-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f164b-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "vendorId": "id-value",
  "vendorNumber": "50000",
  "name": "Nod Publishers",
  "currencyCode": "USD",
  "balanceDue": 17273.87,
  "currentAmount": 0,
  "period1Amount": 0,
  "period2Amount": 0,
  "period3Amount": 17273.87,
  "agedAsOfDate": "2019-01-01",
  "periodLengthFilter": "3M"  
}
```
