---
title: Тип ресурса Триалбаланце
description: Объект пробного баланса в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534852"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="b69cb-103">Тип ресурса Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="b69cb-103">trialBalance resource type</span></span>
<span data-ttu-id="b69cb-104">Представляет пробный баланс в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b69cb-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b69cb-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b69cb-105">Methods</span></span>

| <span data-ttu-id="b69cb-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b69cb-106">Method</span></span>       | <span data-ttu-id="b69cb-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b69cb-107">Return Type</span></span>  |<span data-ttu-id="b69cb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b69cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b69cb-109">Получение Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="b69cb-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="b69cb-110">Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="b69cb-110">trialBalance</span></span>|<span data-ttu-id="b69cb-111">Получает объект пробного баланса.</span><span class="sxs-lookup"><span data-stu-id="b69cb-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b69cb-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="b69cb-112">Properties</span></span>
| <span data-ttu-id="b69cb-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="b69cb-113">Property</span></span>     | <span data-ttu-id="b69cb-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b69cb-114">Type</span></span>   |<span data-ttu-id="b69cb-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b69cb-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b69cb-116">число</span><span class="sxs-lookup"><span data-stu-id="b69cb-116">number</span></span>|<span data-ttu-id="b69cb-117">string</span><span class="sxs-lookup"><span data-stu-id="b69cb-117">string</span></span>|<span data-ttu-id="b69cb-118">Номер финансового счета для элемента Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="b69cb-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="b69cb-119">accountId</span><span class="sxs-lookup"><span data-stu-id="b69cb-119">accountId</span></span>|<span data-ttu-id="b69cb-120">Глобальный уникальный идентификатор (GUID)</span><span class="sxs-lookup"><span data-stu-id="b69cb-120">GUID</span></span>|<span data-ttu-id="b69cb-121">Уникальный идентификатор финансового счета записи.</span><span class="sxs-lookup"><span data-stu-id="b69cb-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="b69cb-122">accountType</span><span class="sxs-lookup"><span data-stu-id="b69cb-122">accountType</span></span>|<span data-ttu-id="b69cb-123">string</span><span class="sxs-lookup"><span data-stu-id="b69cb-123">string</span></span>|<span data-ttu-id="b69cb-124">Тип учетной записи финансового счета записи.</span><span class="sxs-lookup"><span data-stu-id="b69cb-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="b69cb-125">отображения</span><span class="sxs-lookup"><span data-stu-id="b69cb-125">display</span></span>|<span data-ttu-id="b69cb-126">string</span><span class="sxs-lookup"><span data-stu-id="b69cb-126">string</span></span>|<span data-ttu-id="b69cb-127">Имя финансового счета для элемента Триалбаланце.</span><span class="sxs-lookup"><span data-stu-id="b69cb-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="b69cb-128">Тоталдебит</span><span class="sxs-lookup"><span data-stu-id="b69cb-128">totalDebit</span></span>|<span data-ttu-id="b69cb-129">string</span><span class="sxs-lookup"><span data-stu-id="b69cb-129">string</span></span>|<span data-ttu-id="b69cb-130">Представляет общую сумму дебета в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="b69cb-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="b69cb-131">Тоталкредит</span><span class="sxs-lookup"><span data-stu-id="b69cb-131">totalCredit</span></span>|<span data-ttu-id="b69cb-132">string</span><span class="sxs-lookup"><span data-stu-id="b69cb-132">string</span></span>|<span data-ttu-id="b69cb-133">Представляет общую сумму кредита в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="b69cb-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="b69cb-134">Баланцеатдатедебит</span><span class="sxs-lookup"><span data-stu-id="b69cb-134">balanceAtDateDebit</span></span>|<span data-ttu-id="b69cb-135">string</span><span class="sxs-lookup"><span data-stu-id="b69cb-135">string</span></span>|<span data-ttu-id="b69cb-136">Представляет положительное сальдо на сумму даты в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="b69cb-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="b69cb-137">Баланцеатдатекредит</span><span class="sxs-lookup"><span data-stu-id="b69cb-137">balanceAtDateCredit</span></span>|<span data-ttu-id="b69cb-138">string</span><span class="sxs-lookup"><span data-stu-id="b69cb-138">string</span></span>|<span data-ttu-id="b69cb-139">Представляет отрицательное сальдо на сумму даты в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="b69cb-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="b69cb-140">Датефилтер</span><span class="sxs-lookup"><span data-stu-id="b69cb-140">dateFilter</span></span>|<span data-ttu-id="b69cb-141">дата</span><span class="sxs-lookup"><span data-stu-id="b69cb-141">date</span></span>|<span data-ttu-id="b69cb-142">Фильтр даты, используемый для вычисления элементов Триалбаланце.</span><span class="sxs-lookup"><span data-stu-id="b69cb-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b69cb-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="b69cb-143">Relationships</span></span>
<span data-ttu-id="b69cb-144">Нет</span><span class="sxs-lookup"><span data-stu-id="b69cb-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b69cb-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b69cb-145">JSON representation</span></span>

<span data-ttu-id="b69cb-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b69cb-146">Here is a JSON representation of the resource.</span></span>


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```

