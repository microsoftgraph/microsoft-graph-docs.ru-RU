---
title: Тип ресурса Пайменттермс
description: Объект условий оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365642"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="6496a-103">Тип ресурса Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6496a-103">paymentTerms resource type</span></span>
<span data-ttu-id="6496a-104">Представляет термин платежа в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="6496a-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="6496a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6496a-105">Methods</span></span>

| <span data-ttu-id="6496a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6496a-106">Method</span></span>                                                      | <span data-ttu-id="6496a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6496a-107">Return Type</span></span>|<span data-ttu-id="6496a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6496a-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="6496a-109">Получение Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6496a-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="6496a-110">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6496a-110">paymentTerms</span></span>|<span data-ttu-id="6496a-111">Получение объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="6496a-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="6496a-112">POST Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6496a-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="6496a-113">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6496a-113">paymentTerms</span></span>|<span data-ttu-id="6496a-114">Создайте объект формулы оплаты.</span><span class="sxs-lookup"><span data-stu-id="6496a-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="6496a-115">Исправление Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6496a-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="6496a-116">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6496a-116">paymentTerms</span></span>|<span data-ttu-id="6496a-117">Обновление объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="6496a-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="6496a-118">Удаление Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="6496a-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="6496a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6496a-119">none</span></span>        |<span data-ttu-id="6496a-120">Удаление объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="6496a-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6496a-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="6496a-121">Properties</span></span>
| <span data-ttu-id="6496a-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="6496a-122">Property</span></span>                     | <span data-ttu-id="6496a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6496a-123">Type</span></span>     |<span data-ttu-id="6496a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6496a-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="6496a-125">id</span><span class="sxs-lookup"><span data-stu-id="6496a-125">id</span></span>                            |<span data-ttu-id="6496a-126">GUID</span><span class="sxs-lookup"><span data-stu-id="6496a-126">GUID</span></span>    |<span data-ttu-id="6496a-127">Уникальный идентификатор Пайменттермс.</span><span class="sxs-lookup"><span data-stu-id="6496a-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="6496a-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="6496a-128">Non-editable.</span></span>           |
|<span data-ttu-id="6496a-129">code</span><span class="sxs-lookup"><span data-stu-id="6496a-129">code</span></span>                          |<span data-ttu-id="6496a-130">строка</span><span class="sxs-lookup"><span data-stu-id="6496a-130">string</span></span>  |<span data-ttu-id="6496a-131">Определяет код условия платежа.</span><span class="sxs-lookup"><span data-stu-id="6496a-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="6496a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6496a-132">displayName</span></span>                   |<span data-ttu-id="6496a-133">строка</span><span class="sxs-lookup"><span data-stu-id="6496a-133">string</span></span>  |<span data-ttu-id="6496a-134">Задает отображаемое имя условия платежа.</span><span class="sxs-lookup"><span data-stu-id="6496a-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="6496a-135">Дуедатекалкулатион</span><span class="sxs-lookup"><span data-stu-id="6496a-135">dueDateCalculation</span></span>            |<span data-ttu-id="6496a-136">строка</span><span class="sxs-lookup"><span data-stu-id="6496a-136">string</span></span>  |<span data-ttu-id="6496a-137">Указывает формулу, используемую для расчета даты, на которую необходимо выполнить платеж.</span><span class="sxs-lookup"><span data-stu-id="6496a-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="6496a-138">Дискаунтдатекалкулатион</span><span class="sxs-lookup"><span data-stu-id="6496a-138">discountDateCalculation</span></span>       |<span data-ttu-id="6496a-139">строка</span><span class="sxs-lookup"><span data-stu-id="6496a-139">string</span></span>  |<span data-ttu-id="6496a-140">Указывает формулу, используемую для расчета даты, которую необходимо выполнить для получения скидки.</span><span class="sxs-lookup"><span data-stu-id="6496a-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="6496a-141">Дискаунтперцент</span><span class="sxs-lookup"><span data-stu-id="6496a-141">discountPercent</span></span>               |<span data-ttu-id="6496a-142">числе</span><span class="sxs-lookup"><span data-stu-id="6496a-142">decimal</span></span> |<span data-ttu-id="6496a-143">Указывает процент скидки, который применяется для раннего платежа по сумме накладной.</span><span class="sxs-lookup"><span data-stu-id="6496a-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="6496a-144">Калкулатедискаунтонкредитмемос</span><span class="sxs-lookup"><span data-stu-id="6496a-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="6496a-145">boolean</span><span class="sxs-lookup"><span data-stu-id="6496a-145">boolean</span></span> |<span data-ttu-id="6496a-146">Указывает, следует ли применять скидку к кредитовым нотам.</span><span class="sxs-lookup"><span data-stu-id="6496a-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="6496a-147">**Значение true** указывает, что будет задана скидка, **значение false** указывает, что скидка не будет задана.</span><span class="sxs-lookup"><span data-stu-id="6496a-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="6496a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6496a-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="6496a-149">отличным</span><span class="sxs-lookup"><span data-stu-id="6496a-149">datetime</span></span>|<span data-ttu-id="6496a-150">Дата и время последнего изменения Пайменттермс.</span><span class="sxs-lookup"><span data-stu-id="6496a-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="6496a-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6496a-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="6496a-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="6496a-152">Relationships</span></span>
<span data-ttu-id="6496a-153">Нет</span><span class="sxs-lookup"><span data-stu-id="6496a-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6496a-154">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6496a-154">JSON representation</span></span>

<span data-ttu-id="6496a-155">Ниже показано представление объекта Пайменттермс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6496a-155">Here is a JSON representation of the paymentTerms.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
