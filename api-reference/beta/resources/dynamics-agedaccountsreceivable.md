---
title: Тип ресурса Ажедаккаунтсрецеивабле
description: Объект устаревших расчетов с клиентами в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 4d56e954e39bae22db07e025f9570f1fe7a92280
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040062"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="abc55-103">Тип ресурса Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="abc55-103">agedAccountsReceivable resource type</span></span>

<span data-ttu-id="abc55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abc55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abc55-105">Представляет объект Ажедаккаунтсрецеивабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи клиента.</span><span class="sxs-lookup"><span data-stu-id="abc55-105">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="abc55-106">Методы</span><span class="sxs-lookup"><span data-stu-id="abc55-106">Methods</span></span>

| <span data-ttu-id="abc55-107">Метод</span><span class="sxs-lookup"><span data-stu-id="abc55-107">Method</span></span>         | <span data-ttu-id="abc55-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="abc55-108">Return Type</span></span>  |<span data-ttu-id="abc55-109">Описание</span><span class="sxs-lookup"><span data-stu-id="abc55-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="abc55-110">Получение Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="abc55-110">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="abc55-111">ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="abc55-111">agedAccountsReceivable</span></span>|<span data-ttu-id="abc55-112">Получение объекта Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="abc55-112">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="abc55-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="abc55-113">Properties</span></span>
| <span data-ttu-id="abc55-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="abc55-114">Property</span></span>       | <span data-ttu-id="abc55-115">Тип</span><span class="sxs-lookup"><span data-stu-id="abc55-115">Type</span></span>    |<span data-ttu-id="abc55-116">Описание</span><span class="sxs-lookup"><span data-stu-id="abc55-116">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="abc55-117">customerId</span><span class="sxs-lookup"><span data-stu-id="abc55-117">customerId</span></span>      |<span data-ttu-id="abc55-118">GUID</span><span class="sxs-lookup"><span data-stu-id="abc55-118">GUID</span></span>     |<span data-ttu-id="abc55-119">Уникальный идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="abc55-119">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="abc55-120">кустомернумбер</span><span class="sxs-lookup"><span data-stu-id="abc55-120">customerNumber</span></span>  |<span data-ttu-id="abc55-121">string</span><span class="sxs-lookup"><span data-stu-id="abc55-121">string</span></span>   |<span data-ttu-id="abc55-122">Указывает номер клиента.</span><span class="sxs-lookup"><span data-stu-id="abc55-122">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="abc55-123">name</span><span class="sxs-lookup"><span data-stu-id="abc55-123">name</span></span>            |<span data-ttu-id="abc55-124">string</span><span class="sxs-lookup"><span data-stu-id="abc55-124">string</span></span>   |<span data-ttu-id="abc55-125">Указывает имя клиента.</span><span class="sxs-lookup"><span data-stu-id="abc55-125">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="abc55-126">курренцикоде</span><span class="sxs-lookup"><span data-stu-id="abc55-126">currencyCode</span></span>    |<span data-ttu-id="abc55-127">string</span><span class="sxs-lookup"><span data-stu-id="abc55-127">string</span></span>   |<span data-ttu-id="abc55-128">Задает валюту.</span><span class="sxs-lookup"><span data-stu-id="abc55-128">Specifies the currency.</span></span>                      |
|<span data-ttu-id="abc55-129">баланцедуе</span><span class="sxs-lookup"><span data-stu-id="abc55-129">balanceDue</span></span>      |<span data-ttu-id="abc55-130">числовых</span><span class="sxs-lookup"><span data-stu-id="abc55-130">numeric</span></span>  |<span data-ttu-id="abc55-131">Указывает общее сальдо клиента.</span><span class="sxs-lookup"><span data-stu-id="abc55-131">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="abc55-132">куррентамаунт</span><span class="sxs-lookup"><span data-stu-id="abc55-132">currentAmount</span></span>   |<span data-ttu-id="abc55-133">числовых</span><span class="sxs-lookup"><span data-stu-id="abc55-133">numeric</span></span>  |<span data-ttu-id="abc55-134">Указывает баланс для текущего периода распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="abc55-134">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="abc55-135">period1Amount</span><span class="sxs-lookup"><span data-stu-id="abc55-135">period1Amount</span></span>   |<span data-ttu-id="abc55-136">числовых</span><span class="sxs-lookup"><span data-stu-id="abc55-136">numeric</span></span>  |<span data-ttu-id="abc55-137">Указывает баланс в первом периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="abc55-137">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="abc55-138">period2Amount</span><span class="sxs-lookup"><span data-stu-id="abc55-138">period2Amount</span></span>   |<span data-ttu-id="abc55-139">числовых</span><span class="sxs-lookup"><span data-stu-id="abc55-139">numeric</span></span>  |<span data-ttu-id="abc55-140">Указывает баланс во втором периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="abc55-140">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="abc55-141">period3Amount</span><span class="sxs-lookup"><span data-stu-id="abc55-141">period3Amount</span></span>   |<span data-ttu-id="abc55-142">числовых</span><span class="sxs-lookup"><span data-stu-id="abc55-142">numeric</span></span>  |<span data-ttu-id="abc55-143">Указывает баланс в третьем периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="abc55-143">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="abc55-144">ажедасофдате</span><span class="sxs-lookup"><span data-stu-id="abc55-144">agedAsOfDate</span></span>    |<span data-ttu-id="abc55-145">date</span><span class="sxs-lookup"><span data-stu-id="abc55-145">date</span></span>     |<span data-ttu-id="abc55-146">Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="abc55-146">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="abc55-147">периодленгсфилтер</span><span class="sxs-lookup"><span data-stu-id="abc55-147">periodLengthFilter</span></span>|<span data-ttu-id="abc55-148">string</span><span class="sxs-lookup"><span data-stu-id="abc55-148">string</span></span> |<span data-ttu-id="abc55-149">Указывает длину периодов.</span><span class="sxs-lookup"><span data-stu-id="abc55-149">Specifies the length of the periods.</span></span> <span data-ttu-id="abc55-150">Допустимые единицы времени: D, WD, W, M, Q и Y. C, то есть текущая единица времени на основе даты может указываться в качестве префикса для единицы времени.</span><span class="sxs-lookup"><span data-stu-id="abc55-150">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="abc55-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="abc55-151">Relationships</span></span>
<span data-ttu-id="abc55-152">Нет</span><span class="sxs-lookup"><span data-stu-id="abc55-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="abc55-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="abc55-153">JSON representation</span></span>

<span data-ttu-id="abc55-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abc55-154">Here is a JSON representation of the resource.</span></span>


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```




