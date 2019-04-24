---
title: Тип ресурса Ажедаккаунтсрецеивабле
description: Объект устаревших расчетов с клиентами в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507618"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="5937f-103">Тип ресурса Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="5937f-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="5937f-104">Представляет объект Ажедаккаунтсрецеивабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи клиента.</span><span class="sxs-lookup"><span data-stu-id="5937f-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="5937f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5937f-105">Methods</span></span>

| <span data-ttu-id="5937f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5937f-106">Method</span></span>         | <span data-ttu-id="5937f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5937f-107">Return Type</span></span>  |<span data-ttu-id="5937f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5937f-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="5937f-109">Получение Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="5937f-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="5937f-110">Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="5937f-110">agedAccountsReceivable</span></span>|<span data-ttu-id="5937f-111">Получение объекта Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="5937f-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="5937f-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="5937f-112">Properties</span></span>
| <span data-ttu-id="5937f-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="5937f-113">Property</span></span>       | <span data-ttu-id="5937f-114">Тип</span><span class="sxs-lookup"><span data-stu-id="5937f-114">Type</span></span>    |<span data-ttu-id="5937f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="5937f-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="5937f-116">customerId</span><span class="sxs-lookup"><span data-stu-id="5937f-116">customerId</span></span>      |<span data-ttu-id="5937f-117">GUID</span><span class="sxs-lookup"><span data-stu-id="5937f-117">GUID</span></span>     |<span data-ttu-id="5937f-118">Уникальный идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="5937f-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="5937f-119">Кустомернумбер</span><span class="sxs-lookup"><span data-stu-id="5937f-119">customerNumber</span></span>  |<span data-ttu-id="5937f-120">строка</span><span class="sxs-lookup"><span data-stu-id="5937f-120">string</span></span>   |<span data-ttu-id="5937f-121">Указывает номер клиента.</span><span class="sxs-lookup"><span data-stu-id="5937f-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="5937f-122">name</span><span class="sxs-lookup"><span data-stu-id="5937f-122">name</span></span>            |<span data-ttu-id="5937f-123">string</span><span class="sxs-lookup"><span data-stu-id="5937f-123">string</span></span>   |<span data-ttu-id="5937f-124">Указывает имя клиента.</span><span class="sxs-lookup"><span data-stu-id="5937f-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="5937f-125">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="5937f-125">currencyCode</span></span>    |<span data-ttu-id="5937f-126">строка</span><span class="sxs-lookup"><span data-stu-id="5937f-126">string</span></span>   |<span data-ttu-id="5937f-127">Задает валюту.</span><span class="sxs-lookup"><span data-stu-id="5937f-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="5937f-128">Баланцедуе</span><span class="sxs-lookup"><span data-stu-id="5937f-128">balanceDue</span></span>      |<span data-ttu-id="5937f-129">числовых</span><span class="sxs-lookup"><span data-stu-id="5937f-129">numeric</span></span>  |<span data-ttu-id="5937f-130">Указывает общее сальдо клиента.</span><span class="sxs-lookup"><span data-stu-id="5937f-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="5937f-131">Куррентамаунт</span><span class="sxs-lookup"><span data-stu-id="5937f-131">currentAmount</span></span>   |<span data-ttu-id="5937f-132">числовых</span><span class="sxs-lookup"><span data-stu-id="5937f-132">numeric</span></span>  |<span data-ttu-id="5937f-133">Указывает баланс для текущего периода распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="5937f-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="5937f-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="5937f-134">period1Amount</span></span>   |<span data-ttu-id="5937f-135">числовых</span><span class="sxs-lookup"><span data-stu-id="5937f-135">numeric</span></span>  |<span data-ttu-id="5937f-136">Указывает баланс в первом периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="5937f-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="5937f-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="5937f-137">period2Amount</span></span>   |<span data-ttu-id="5937f-138">числовых</span><span class="sxs-lookup"><span data-stu-id="5937f-138">numeric</span></span>  |<span data-ttu-id="5937f-139">Указывает баланс во втором периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="5937f-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="5937f-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="5937f-140">period3Amount</span></span>   |<span data-ttu-id="5937f-141">числовых</span><span class="sxs-lookup"><span data-stu-id="5937f-141">numeric</span></span>  |<span data-ttu-id="5937f-142">Указывает баланс в третьем периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="5937f-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="5937f-143">Ажедасофдате</span><span class="sxs-lookup"><span data-stu-id="5937f-143">agedAsOfDate</span></span>    |<span data-ttu-id="5937f-144">дата</span><span class="sxs-lookup"><span data-stu-id="5937f-144">date</span></span>     |<span data-ttu-id="5937f-145">Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="5937f-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="5937f-146">Периодленгсфилтер</span><span class="sxs-lookup"><span data-stu-id="5937f-146">periodLengthFilter</span></span>|<span data-ttu-id="5937f-147">строка</span><span class="sxs-lookup"><span data-stu-id="5937f-147">string</span></span> |<span data-ttu-id="5937f-148">Указывает длину периодов.</span><span class="sxs-lookup"><span data-stu-id="5937f-148">Specifies the length of the periods.</span></span> <span data-ttu-id="5937f-149">Допустимые единицы времени: D, WD, W, M, Q и Y. C, то есть текущая единица времени на основе даты может указываться в качестве префикса для единицы времени.</span><span class="sxs-lookup"><span data-stu-id="5937f-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="5937f-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="5937f-150">Relationships</span></span>
<span data-ttu-id="5937f-151">Нет</span><span class="sxs-lookup"><span data-stu-id="5937f-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5937f-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5937f-152">JSON representation</span></span>

<span data-ttu-id="5937f-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5937f-153">Here is a JSON representation of the resource.</span></span>


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


