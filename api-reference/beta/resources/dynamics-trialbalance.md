---
title: Тип ресурса Триалбаланце
description: Объект пробного баланса в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: b7d3fee76df5f60c47639183f7d3e7ce54164f81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503217"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="2aa2d-103">Тип ресурса Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="2aa2d-103">trialBalance resource type</span></span>

<span data-ttu-id="2aa2d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2aa2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2aa2d-105">Представляет пробный баланс в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-105">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="2aa2d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2aa2d-106">Methods</span></span>

| <span data-ttu-id="2aa2d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2aa2d-107">Method</span></span>       | <span data-ttu-id="2aa2d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2aa2d-108">Return Type</span></span>  |<span data-ttu-id="2aa2d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2aa2d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2aa2d-110">Получение Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="2aa2d-110">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="2aa2d-111">триалбаланце</span><span class="sxs-lookup"><span data-stu-id="2aa2d-111">trialBalance</span></span>|<span data-ttu-id="2aa2d-112">Получает объект пробного баланса.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-112">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2aa2d-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="2aa2d-113">Properties</span></span>
| <span data-ttu-id="2aa2d-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="2aa2d-114">Property</span></span>     | <span data-ttu-id="2aa2d-115">Тип</span><span class="sxs-lookup"><span data-stu-id="2aa2d-115">Type</span></span>   |<span data-ttu-id="2aa2d-116">Описание</span><span class="sxs-lookup"><span data-stu-id="2aa2d-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2aa2d-117">число</span><span class="sxs-lookup"><span data-stu-id="2aa2d-117">number</span></span>|<span data-ttu-id="2aa2d-118">строка</span><span class="sxs-lookup"><span data-stu-id="2aa2d-118">string</span></span>|<span data-ttu-id="2aa2d-119">Номер финансового счета для элемента Триалбаланце</span><span class="sxs-lookup"><span data-stu-id="2aa2d-119">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="2aa2d-120">accountId</span><span class="sxs-lookup"><span data-stu-id="2aa2d-120">accountId</span></span>|<span data-ttu-id="2aa2d-121">GUID</span><span class="sxs-lookup"><span data-stu-id="2aa2d-121">GUID</span></span>|<span data-ttu-id="2aa2d-122">Уникальный идентификатор финансового счета записи.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-122">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="2aa2d-123">accountType</span><span class="sxs-lookup"><span data-stu-id="2aa2d-123">accountType</span></span>|<span data-ttu-id="2aa2d-124">строка</span><span class="sxs-lookup"><span data-stu-id="2aa2d-124">string</span></span>|<span data-ttu-id="2aa2d-125">Тип учетной записи финансового счета записи.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-125">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="2aa2d-126">отображения</span><span class="sxs-lookup"><span data-stu-id="2aa2d-126">display</span></span>|<span data-ttu-id="2aa2d-127">строка</span><span class="sxs-lookup"><span data-stu-id="2aa2d-127">string</span></span>|<span data-ttu-id="2aa2d-128">Имя финансового счета для элемента Триалбаланце.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-128">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="2aa2d-129">тоталдебит</span><span class="sxs-lookup"><span data-stu-id="2aa2d-129">totalDebit</span></span>|<span data-ttu-id="2aa2d-130">строка</span><span class="sxs-lookup"><span data-stu-id="2aa2d-130">string</span></span>|<span data-ttu-id="2aa2d-131">Представляет общую сумму дебета в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-131">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="2aa2d-132">тоталкредит</span><span class="sxs-lookup"><span data-stu-id="2aa2d-132">totalCredit</span></span>|<span data-ttu-id="2aa2d-133">строка</span><span class="sxs-lookup"><span data-stu-id="2aa2d-133">string</span></span>|<span data-ttu-id="2aa2d-134">Представляет общую сумму кредита в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-134">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="2aa2d-135">баланцеатдатедебит</span><span class="sxs-lookup"><span data-stu-id="2aa2d-135">balanceAtDateDebit</span></span>|<span data-ttu-id="2aa2d-136">строка</span><span class="sxs-lookup"><span data-stu-id="2aa2d-136">string</span></span>|<span data-ttu-id="2aa2d-137">Представляет положительное сальдо на сумму даты в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-137">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="2aa2d-138">баланцеатдатекредит</span><span class="sxs-lookup"><span data-stu-id="2aa2d-138">balanceAtDateCredit</span></span>|<span data-ttu-id="2aa2d-139">строка</span><span class="sxs-lookup"><span data-stu-id="2aa2d-139">string</span></span>|<span data-ttu-id="2aa2d-140">Представляет отрицательное сальдо на сумму даты в финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-140">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="2aa2d-141">датефилтер</span><span class="sxs-lookup"><span data-stu-id="2aa2d-141">dateFilter</span></span>|<span data-ttu-id="2aa2d-142">date</span><span class="sxs-lookup"><span data-stu-id="2aa2d-142">date</span></span>|<span data-ttu-id="2aa2d-143">Фильтр даты, используемый для вычисления элементов Триалбаланце.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-143">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2aa2d-144">Связи</span><span class="sxs-lookup"><span data-stu-id="2aa2d-144">Relationships</span></span>
<span data-ttu-id="2aa2d-145">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa2d-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2aa2d-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2aa2d-146">JSON representation</span></span>

<span data-ttu-id="2aa2d-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aa2d-147">Here is a JSON representation of the resource.</span></span>


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

