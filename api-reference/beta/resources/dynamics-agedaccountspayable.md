---
title: Тип ресурса Ажедаккаунтспайабле
description: Объект кредиторской задолженности в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 9a8dc7eed4bdbcc39a04f55996e11b6d9dc6da1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505170"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="cca90-103">Тип ресурса Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="cca90-103">agedAccountsPayable resource type</span></span>

<span data-ttu-id="cca90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cca90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cca90-105">Представляет объект Ажедаккаунтспайабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи поставщика.</span><span class="sxs-lookup"><span data-stu-id="cca90-105">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="cca90-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cca90-106">Methods</span></span>

| <span data-ttu-id="cca90-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cca90-107">Method</span></span>         | <span data-ttu-id="cca90-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cca90-108">Return Type</span></span>  |<span data-ttu-id="cca90-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cca90-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="cca90-110">Получение Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="cca90-110">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="cca90-111">ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="cca90-111">agedAccountsPayable</span></span>|<span data-ttu-id="cca90-112">Получение объекта Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="cca90-112">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="cca90-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="cca90-113">Properties</span></span>
| <span data-ttu-id="cca90-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="cca90-114">Property</span></span>      | <span data-ttu-id="cca90-115">Тип</span><span class="sxs-lookup"><span data-stu-id="cca90-115">Type</span></span>     |<span data-ttu-id="cca90-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cca90-116">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="cca90-117">Поставщика</span><span class="sxs-lookup"><span data-stu-id="cca90-117">vendorId</span></span>       |<span data-ttu-id="cca90-118">GUID</span><span class="sxs-lookup"><span data-stu-id="cca90-118">GUID</span></span>      |<span data-ttu-id="cca90-119">Уникальный идентификатор поставщика.</span><span class="sxs-lookup"><span data-stu-id="cca90-119">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="cca90-120">вендорнумбер</span><span class="sxs-lookup"><span data-stu-id="cca90-120">vendorNumber</span></span>   |<span data-ttu-id="cca90-121">string</span><span class="sxs-lookup"><span data-stu-id="cca90-121">string</span></span>    |<span data-ttu-id="cca90-122">Указывает номер поставщика.</span><span class="sxs-lookup"><span data-stu-id="cca90-122">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="cca90-123">name</span><span class="sxs-lookup"><span data-stu-id="cca90-123">name</span></span>           |<span data-ttu-id="cca90-124">string</span><span class="sxs-lookup"><span data-stu-id="cca90-124">string</span></span>    |<span data-ttu-id="cca90-125">Указывает имя поставщика.</span><span class="sxs-lookup"><span data-stu-id="cca90-125">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="cca90-126">курренцикоде</span><span class="sxs-lookup"><span data-stu-id="cca90-126">currencyCode</span></span>   |<span data-ttu-id="cca90-127">string</span><span class="sxs-lookup"><span data-stu-id="cca90-127">string</span></span>    |<span data-ttu-id="cca90-128">Задает валюту.</span><span class="sxs-lookup"><span data-stu-id="cca90-128">Specifies the currency.</span></span>                     |
|<span data-ttu-id="cca90-129">баланцедуе</span><span class="sxs-lookup"><span data-stu-id="cca90-129">balanceDue</span></span>     |<span data-ttu-id="cca90-130">числовых</span><span class="sxs-lookup"><span data-stu-id="cca90-130">numeric</span></span>   |<span data-ttu-id="cca90-131">Указывает общее сальдо, которое связано с поставщиком.</span><span class="sxs-lookup"><span data-stu-id="cca90-131">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="cca90-132">куррентамаунт</span><span class="sxs-lookup"><span data-stu-id="cca90-132">currentAmount</span></span>  |<span data-ttu-id="cca90-133">числовых</span><span class="sxs-lookup"><span data-stu-id="cca90-133">numeric</span></span>   |<span data-ttu-id="cca90-134">Указывает баланс перед первым периодом распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="cca90-134">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="cca90-135">period1Amount</span><span class="sxs-lookup"><span data-stu-id="cca90-135">period1Amount</span></span>  |<span data-ttu-id="cca90-136">числовых</span><span class="sxs-lookup"><span data-stu-id="cca90-136">numeric</span></span>   |<span data-ttu-id="cca90-137">Указывает баланс в первом периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="cca90-137">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="cca90-138">period2Amount</span><span class="sxs-lookup"><span data-stu-id="cca90-138">period2Amount</span></span>  |<span data-ttu-id="cca90-139">числовых</span><span class="sxs-lookup"><span data-stu-id="cca90-139">numeric</span></span>   |<span data-ttu-id="cca90-140">Указывает баланс во втором периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="cca90-140">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="cca90-141">period3Amount</span><span class="sxs-lookup"><span data-stu-id="cca90-141">period3Amount</span></span>  |<span data-ttu-id="cca90-142">числовых</span><span class="sxs-lookup"><span data-stu-id="cca90-142">numeric</span></span>   |<span data-ttu-id="cca90-143">Указывает баланс в третьем периоде распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="cca90-143">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="cca90-144">ажедасофдате</span><span class="sxs-lookup"><span data-stu-id="cca90-144">agedAsOfDate</span></span>   |<span data-ttu-id="cca90-145">date</span><span class="sxs-lookup"><span data-stu-id="cca90-145">date</span></span>|<span data-ttu-id="cca90-146">Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.</span><span class="sxs-lookup"><span data-stu-id="cca90-146">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="cca90-147">периодленгсфилтер</span><span class="sxs-lookup"><span data-stu-id="cca90-147">periodLengthFilter</span></span>|<span data-ttu-id="cca90-148">string</span><span class="sxs-lookup"><span data-stu-id="cca90-148">string</span></span> |<span data-ttu-id="cca90-149">Указывает длину периодов.</span><span class="sxs-lookup"><span data-stu-id="cca90-149">Specifies the length of the periods.</span></span> <span data-ttu-id="cca90-150">Допустимые значения для единиц времени: D, WD, W, M, Q или Y. C, то есть текущая единица времени на основе даты может быть указана в качестве префикса для единицы времени.</span><span class="sxs-lookup"><span data-stu-id="cca90-150">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="cca90-151">Связи</span><span class="sxs-lookup"><span data-stu-id="cca90-151">Relationships</span></span>
<span data-ttu-id="cca90-152">Нет</span><span class="sxs-lookup"><span data-stu-id="cca90-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cca90-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cca90-153">JSON representation</span></span>

<span data-ttu-id="cca90-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cca90-154">Here is a JSON representation of the resource.</span></span>


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
