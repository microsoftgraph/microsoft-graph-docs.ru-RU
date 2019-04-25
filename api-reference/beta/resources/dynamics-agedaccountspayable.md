---
title: Тип ресурса Ажедаккаунтспайабле
description: Объект кредиторской задолженности в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543135"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="601bf-103">Тип ресурса Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="601bf-103">agedAccountsPayable resource type</span></span>
<span data-ttu-id="601bf-104">Представляет объект Ажедаккаунтспайабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи поставщика.</span><span class="sxs-lookup"><span data-stu-id="601bf-104">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="601bf-105">Методы</span><span class="sxs-lookup"><span data-stu-id="601bf-105">Methods</span></span>

| <span data-ttu-id="601bf-106">Метод</span><span class="sxs-lookup"><span data-stu-id="601bf-106">Method</span></span>         | <span data-ttu-id="601bf-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="601bf-107">Return Type</span></span>  |<span data-ttu-id="601bf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="601bf-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="601bf-109">Получение Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="601bf-109">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="601bf-110">Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="601bf-110">agedAccountsPayable</span></span>|<span data-ttu-id="601bf-111">Получение объекта Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="601bf-111">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="601bf-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="601bf-112">Properties</span></span>
| <span data-ttu-id="601bf-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="601bf-113">Property</span></span>      | <span data-ttu-id="601bf-114">Тип</span><span class="sxs-lookup"><span data-stu-id="601bf-114">Type</span></span>     |<span data-ttu-id="601bf-115">Описание</span><span class="sxs-lookup"><span data-stu-id="601bf-115">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="601bf-116">Поставщика</span><span class="sxs-lookup"><span data-stu-id="601bf-116">vendorId</span></span>       |<span data-ttu-id="601bf-117">Глобальный уникальный идентификатор (GUID)</span><span class="sxs-lookup"><span data-stu-id="601bf-117">GUID</span></span>      |<span data-ttu-id="601bf-118">Уникальный идентификатор поставщика.</span><span class="sxs-lookup"><span data-stu-id="601bf-118">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="601bf-119">Вендорнумбер</span><span class="sxs-lookup"><span data-stu-id="601bf-119">vendorNumber</span></span>   |<span data-ttu-id="601bf-120">string</span><span class="sxs-lookup"><span data-stu-id="601bf-120">string</span></span>    |<span data-ttu-id="601bf-121">Указывает номер поставщика.</span><span class="sxs-lookup"><span data-stu-id="601bf-121">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="601bf-122">name</span><span class="sxs-lookup"><span data-stu-id="601bf-122">name</span></span>           |<span data-ttu-id="601bf-123">string</span><span class="sxs-lookup"><span data-stu-id="601bf-123">string</span></span>    |<span data-ttu-id="601bf-124">Указывает имя поставщика.</span><span class="sxs-lookup"><span data-stu-id="601bf-124">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="601bf-125">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="601bf-125">currencyCode</span></span>   |<span data-ttu-id="601bf-126">string</span><span class="sxs-lookup"><span data-stu-id="601bf-126">string</span></span>    |<span data-ttu-id="601bf-127">Задает валюту.</span><span class="sxs-lookup"><span data-stu-id="601bf-127">Specifies the currency.</span></span>                     |
|<span data-ttu-id="601bf-128">Баланцедуе</span><span class="sxs-lookup"><span data-stu-id="601bf-128">balanceDue</span></span>     |<span data-ttu-id="601bf-129">числовых</span><span class="sxs-lookup"><span data-stu-id="601bf-129">numeric</span></span>   |<span data-ttu-id="601bf-130">Указывает общее сальдо, которое связано с поставщиком.</span><span class="sxs-lookup"><span data-stu-id="601bf-130">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="601bf-131">Куррентамаунт</span><span class="sxs-lookup"><span data-stu-id="601bf-131">currentAmount</span></span>  |<span data-ttu-id="601bf-132">числовых</span><span class="sxs-lookup"><span data-stu-id="601bf-132">numeric</span></span>   |<span data-ttu-id="601bf-133">Указывает баланс перед первым периодом распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="601bf-133">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="601bf-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="601bf-134">period1Amount</span></span>  |<span data-ttu-id="601bf-135">числовых</span><span class="sxs-lookup"><span data-stu-id="601bf-135">numeric</span></span>   |<span data-ttu-id="601bf-136">Указывает баланс в первом периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="601bf-136">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="601bf-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="601bf-137">period2Amount</span></span>  |<span data-ttu-id="601bf-138">числовых</span><span class="sxs-lookup"><span data-stu-id="601bf-138">numeric</span></span>   |<span data-ttu-id="601bf-139">Указывает баланс во втором периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="601bf-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="601bf-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="601bf-140">period3Amount</span></span>  |<span data-ttu-id="601bf-141">числовых</span><span class="sxs-lookup"><span data-stu-id="601bf-141">numeric</span></span>   |<span data-ttu-id="601bf-142">Указывает баланс в третьем периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="601bf-142">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="601bf-143">Ажедасофдате</span><span class="sxs-lookup"><span data-stu-id="601bf-143">agedAsOfDate</span></span>   |<span data-ttu-id="601bf-144">дата</span><span class="sxs-lookup"><span data-stu-id="601bf-144">date</span></span>|<span data-ttu-id="601bf-145">Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="601bf-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="601bf-146">Периодленгсфилтер</span><span class="sxs-lookup"><span data-stu-id="601bf-146">periodLengthFilter</span></span>|<span data-ttu-id="601bf-147">string</span><span class="sxs-lookup"><span data-stu-id="601bf-147">string</span></span> |<span data-ttu-id="601bf-148">Указывает длину периодов.</span><span class="sxs-lookup"><span data-stu-id="601bf-148">Specifies the length of the periods.</span></span> <span data-ttu-id="601bf-149">Допустимые значения для единиц времени: D, WD, W, M, Q или Y. C, то есть текущая единица времени на основе даты может быть указана в качестве префикса для единицы времени.</span><span class="sxs-lookup"><span data-stu-id="601bf-149">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="601bf-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="601bf-150">Relationships</span></span>
<span data-ttu-id="601bf-151">Нет</span><span class="sxs-lookup"><span data-stu-id="601bf-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="601bf-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="601bf-152">JSON representation</span></span>

<span data-ttu-id="601bf-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="601bf-153">Here is a JSON representation of the resource.</span></span>


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
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
