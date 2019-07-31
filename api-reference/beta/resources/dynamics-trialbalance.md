---
title: Тип ресурса Триалбаланце
description: Объект пробного баланса в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 02e4f039411c992cd1d7335fc2463d660b8ff181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972875"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="4af13-103">Тип ресурса Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="4af13-103">trialBalance resource type</span></span>
<span data-ttu-id="4af13-104">Представляет пробный баланс в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="4af13-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="4af13-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4af13-105">Methods</span></span>

| <span data-ttu-id="4af13-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4af13-106">Method</span></span>       | <span data-ttu-id="4af13-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4af13-107">Return Type</span></span>  |<span data-ttu-id="4af13-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4af13-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4af13-109">Получение Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="4af13-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="4af13-110">Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="4af13-110">trialBalance</span></span>|<span data-ttu-id="4af13-111">Получает объект пробного баланса.</span><span class="sxs-lookup"><span data-stu-id="4af13-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4af13-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="4af13-112">Properties</span></span>
| <span data-ttu-id="4af13-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="4af13-113">Property</span></span>     | <span data-ttu-id="4af13-114">Тип</span><span class="sxs-lookup"><span data-stu-id="4af13-114">Type</span></span>   |<span data-ttu-id="4af13-115">Описание</span><span class="sxs-lookup"><span data-stu-id="4af13-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4af13-116">число</span><span class="sxs-lookup"><span data-stu-id="4af13-116">number</span></span>|<span data-ttu-id="4af13-117">string</span><span class="sxs-lookup"><span data-stu-id="4af13-117">string</span></span>|<span data-ttu-id="4af13-118">Номер финансового счета для элемента Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="4af13-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="4af13-119">accountId</span><span class="sxs-lookup"><span data-stu-id="4af13-119">accountId</span></span>|<span data-ttu-id="4af13-120">GUID</span><span class="sxs-lookup"><span data-stu-id="4af13-120">GUID</span></span>|<span data-ttu-id="4af13-121">Уникальный идентификатор финансового счета записи.</span><span class="sxs-lookup"><span data-stu-id="4af13-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="4af13-122">accountType</span><span class="sxs-lookup"><span data-stu-id="4af13-122">accountType</span></span>|<span data-ttu-id="4af13-123">string</span><span class="sxs-lookup"><span data-stu-id="4af13-123">string</span></span>|<span data-ttu-id="4af13-124">Тип учетной записи финансового счета записи.</span><span class="sxs-lookup"><span data-stu-id="4af13-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="4af13-125">отображения</span><span class="sxs-lookup"><span data-stu-id="4af13-125">display</span></span>|<span data-ttu-id="4af13-126">string</span><span class="sxs-lookup"><span data-stu-id="4af13-126">string</span></span>|<span data-ttu-id="4af13-127">Имя финансового счета для элемента Триалбаланце.</span><span class="sxs-lookup"><span data-stu-id="4af13-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="4af13-128">Тоталдебит</span><span class="sxs-lookup"><span data-stu-id="4af13-128">totalDebit</span></span>|<span data-ttu-id="4af13-129">string</span><span class="sxs-lookup"><span data-stu-id="4af13-129">string</span></span>|<span data-ttu-id="4af13-130">Представляет общую сумму дебета в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="4af13-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="4af13-131">Тоталкредит</span><span class="sxs-lookup"><span data-stu-id="4af13-131">totalCredit</span></span>|<span data-ttu-id="4af13-132">string</span><span class="sxs-lookup"><span data-stu-id="4af13-132">string</span></span>|<span data-ttu-id="4af13-133">Представляет общую сумму кредита в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="4af13-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="4af13-134">Баланцеатдатедебит</span><span class="sxs-lookup"><span data-stu-id="4af13-134">balanceAtDateDebit</span></span>|<span data-ttu-id="4af13-135">string</span><span class="sxs-lookup"><span data-stu-id="4af13-135">string</span></span>|<span data-ttu-id="4af13-136">Представляет положительное сальдо на сумму даты в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="4af13-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="4af13-137">Баланцеатдатекредит</span><span class="sxs-lookup"><span data-stu-id="4af13-137">balanceAtDateCredit</span></span>|<span data-ttu-id="4af13-138">string</span><span class="sxs-lookup"><span data-stu-id="4af13-138">string</span></span>|<span data-ttu-id="4af13-139">Представляет отрицательное сальдо на сумму даты в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="4af13-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="4af13-140">Датефилтер</span><span class="sxs-lookup"><span data-stu-id="4af13-140">dateFilter</span></span>|<span data-ttu-id="4af13-141">date</span><span class="sxs-lookup"><span data-stu-id="4af13-141">date</span></span>|<span data-ttu-id="4af13-142">Фильтр даты, используемый для вычисления элементов Триалбаланце.</span><span class="sxs-lookup"><span data-stu-id="4af13-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4af13-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="4af13-143">Relationships</span></span>
<span data-ttu-id="4af13-144">Нет</span><span class="sxs-lookup"><span data-stu-id="4af13-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4af13-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4af13-145">JSON representation</span></span>

<span data-ttu-id="4af13-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4af13-146">Here is a JSON representation of the resource.</span></span>


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

