---
title: Тип ресурса Ажедаккаунтсрецеивабле
description: Объект устаревших расчетов с клиентами в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f9589cbb4cb380eececdcc7adf7bd5dd682269f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012676"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="e119d-103">Тип ресурса Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="e119d-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="e119d-104">Представляет объект Ажедаккаунтсрецеивабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи клиента.</span><span class="sxs-lookup"><span data-stu-id="e119d-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="e119d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e119d-105">Methods</span></span>

| <span data-ttu-id="e119d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e119d-106">Method</span></span>         | <span data-ttu-id="e119d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e119d-107">Return Type</span></span>  |<span data-ttu-id="e119d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e119d-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="e119d-109">Получение Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="e119d-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="e119d-110">Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="e119d-110">agedAccountsReceivable</span></span>|<span data-ttu-id="e119d-111">Получение объекта Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="e119d-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="e119d-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="e119d-112">Properties</span></span>
| <span data-ttu-id="e119d-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="e119d-113">Property</span></span>       | <span data-ttu-id="e119d-114">Тип</span><span class="sxs-lookup"><span data-stu-id="e119d-114">Type</span></span>    |<span data-ttu-id="e119d-115">Описание</span><span class="sxs-lookup"><span data-stu-id="e119d-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="e119d-116">customerId</span><span class="sxs-lookup"><span data-stu-id="e119d-116">customerId</span></span>      |<span data-ttu-id="e119d-117">GUID</span><span class="sxs-lookup"><span data-stu-id="e119d-117">GUID</span></span>     |<span data-ttu-id="e119d-118">Уникальный идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="e119d-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="e119d-119">Кустомернумбер</span><span class="sxs-lookup"><span data-stu-id="e119d-119">customerNumber</span></span>  |<span data-ttu-id="e119d-120">string</span><span class="sxs-lookup"><span data-stu-id="e119d-120">string</span></span>   |<span data-ttu-id="e119d-121">Указывает номер клиента.</span><span class="sxs-lookup"><span data-stu-id="e119d-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="e119d-122">name</span><span class="sxs-lookup"><span data-stu-id="e119d-122">name</span></span>            |<span data-ttu-id="e119d-123">string</span><span class="sxs-lookup"><span data-stu-id="e119d-123">string</span></span>   |<span data-ttu-id="e119d-124">Указывает имя клиента.</span><span class="sxs-lookup"><span data-stu-id="e119d-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="e119d-125">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="e119d-125">currencyCode</span></span>    |<span data-ttu-id="e119d-126">string</span><span class="sxs-lookup"><span data-stu-id="e119d-126">string</span></span>   |<span data-ttu-id="e119d-127">Задает валюту.</span><span class="sxs-lookup"><span data-stu-id="e119d-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="e119d-128">Баланцедуе</span><span class="sxs-lookup"><span data-stu-id="e119d-128">balanceDue</span></span>      |<span data-ttu-id="e119d-129">числовых</span><span class="sxs-lookup"><span data-stu-id="e119d-129">numeric</span></span>  |<span data-ttu-id="e119d-130">Указывает общее сальдо клиента.</span><span class="sxs-lookup"><span data-stu-id="e119d-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="e119d-131">Куррентамаунт</span><span class="sxs-lookup"><span data-stu-id="e119d-131">currentAmount</span></span>   |<span data-ttu-id="e119d-132">числовых</span><span class="sxs-lookup"><span data-stu-id="e119d-132">numeric</span></span>  |<span data-ttu-id="e119d-133">Указывает баланс для текущего периода распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="e119d-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="e119d-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="e119d-134">period1Amount</span></span>   |<span data-ttu-id="e119d-135">числовых</span><span class="sxs-lookup"><span data-stu-id="e119d-135">numeric</span></span>  |<span data-ttu-id="e119d-136">Указывает баланс в первом периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="e119d-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="e119d-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="e119d-137">period2Amount</span></span>   |<span data-ttu-id="e119d-138">числовых</span><span class="sxs-lookup"><span data-stu-id="e119d-138">numeric</span></span>  |<span data-ttu-id="e119d-139">Указывает баланс во втором периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="e119d-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="e119d-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="e119d-140">period3Amount</span></span>   |<span data-ttu-id="e119d-141">числовых</span><span class="sxs-lookup"><span data-stu-id="e119d-141">numeric</span></span>  |<span data-ttu-id="e119d-142">Указывает баланс в третьем периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="e119d-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="e119d-143">Ажедасофдате</span><span class="sxs-lookup"><span data-stu-id="e119d-143">agedAsOfDate</span></span>    |<span data-ttu-id="e119d-144">date</span><span class="sxs-lookup"><span data-stu-id="e119d-144">date</span></span>     |<span data-ttu-id="e119d-145">Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="e119d-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="e119d-146">Периодленгсфилтер</span><span class="sxs-lookup"><span data-stu-id="e119d-146">periodLengthFilter</span></span>|<span data-ttu-id="e119d-147">string</span><span class="sxs-lookup"><span data-stu-id="e119d-147">string</span></span> |<span data-ttu-id="e119d-148">Указывает длину периодов.</span><span class="sxs-lookup"><span data-stu-id="e119d-148">Specifies the length of the periods.</span></span> <span data-ttu-id="e119d-149">Допустимые единицы времени: D, WD, W, M, Q и Y. C, то есть текущая единица времени на основе даты может указываться в качестве префикса для единицы времени.</span><span class="sxs-lookup"><span data-stu-id="e119d-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e119d-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="e119d-150">Relationships</span></span>
<span data-ttu-id="e119d-151">Нет</span><span class="sxs-lookup"><span data-stu-id="e119d-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e119d-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e119d-152">JSON representation</span></span>

<span data-ttu-id="e119d-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e119d-153">Here is a JSON representation of the resource.</span></span>


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


