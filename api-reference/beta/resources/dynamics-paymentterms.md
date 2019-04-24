---
title: Тип ресурса Пайменттермс
description: Объект условий оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507331"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="2d1ba-103">Тип ресурса Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="2d1ba-103">paymentTerms resource type</span></span>
<span data-ttu-id="2d1ba-104">Представляет термин платежа в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="2d1ba-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2d1ba-105">Methods</span></span>

| <span data-ttu-id="2d1ba-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2d1ba-106">Method</span></span>                                                      | <span data-ttu-id="2d1ba-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2d1ba-107">Return Type</span></span>|<span data-ttu-id="2d1ba-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2d1ba-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="2d1ba-109">Получение Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="2d1ba-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="2d1ba-110">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="2d1ba-110">paymentTerms</span></span>|<span data-ttu-id="2d1ba-111">Получение объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="2d1ba-112">POST Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="2d1ba-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="2d1ba-113">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="2d1ba-113">paymentTerms</span></span>|<span data-ttu-id="2d1ba-114">Создайте объект формулы оплаты.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="2d1ba-115">Исправление Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="2d1ba-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="2d1ba-116">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="2d1ba-116">paymentTerms</span></span>|<span data-ttu-id="2d1ba-117">Обновление объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="2d1ba-118">Удаление Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="2d1ba-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="2d1ba-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2d1ba-119">none</span></span>        |<span data-ttu-id="2d1ba-120">Удаление объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d1ba-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d1ba-121">Properties</span></span>
| <span data-ttu-id="2d1ba-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d1ba-122">Property</span></span>                     | <span data-ttu-id="2d1ba-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2d1ba-123">Type</span></span>     |<span data-ttu-id="2d1ba-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2d1ba-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="2d1ba-125">id</span><span class="sxs-lookup"><span data-stu-id="2d1ba-125">id</span></span>                            |<span data-ttu-id="2d1ba-126">GUID</span><span class="sxs-lookup"><span data-stu-id="2d1ba-126">GUID</span></span>    |<span data-ttu-id="2d1ba-127">Уникальный идентификатор Пайменттермс.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="2d1ba-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-128">Non-editable.</span></span>           |
|<span data-ttu-id="2d1ba-129">code</span><span class="sxs-lookup"><span data-stu-id="2d1ba-129">code</span></span>                          |<span data-ttu-id="2d1ba-130">string</span><span class="sxs-lookup"><span data-stu-id="2d1ba-130">string</span></span>  |<span data-ttu-id="2d1ba-131">Определяет код условия платежа.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="2d1ba-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2d1ba-132">displayName</span></span>                   |<span data-ttu-id="2d1ba-133">string</span><span class="sxs-lookup"><span data-stu-id="2d1ba-133">string</span></span>  |<span data-ttu-id="2d1ba-134">Задает отображаемое имя условия платежа.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="2d1ba-135">Дуедатекалкулатион</span><span class="sxs-lookup"><span data-stu-id="2d1ba-135">dueDateCalculation</span></span>            |<span data-ttu-id="2d1ba-136">строка</span><span class="sxs-lookup"><span data-stu-id="2d1ba-136">string</span></span>  |<span data-ttu-id="2d1ba-137">Указывает формулу, используемую для расчета даты, на которую необходимо выполнить платеж.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="2d1ba-138">Дискаунтдатекалкулатион</span><span class="sxs-lookup"><span data-stu-id="2d1ba-138">discountDateCalculation</span></span>       |<span data-ttu-id="2d1ba-139">строка</span><span class="sxs-lookup"><span data-stu-id="2d1ba-139">string</span></span>  |<span data-ttu-id="2d1ba-140">Указывает формулу, используемую для расчета даты, которую необходимо выполнить для получения скидки.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="2d1ba-141">Дискаунтперцент</span><span class="sxs-lookup"><span data-stu-id="2d1ba-141">discountPercent</span></span>               |<span data-ttu-id="2d1ba-142">числе</span><span class="sxs-lookup"><span data-stu-id="2d1ba-142">decimal</span></span> |<span data-ttu-id="2d1ba-143">Указывает процент скидки, который применяется для раннего платежа по сумме накладной.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="2d1ba-144">Калкулатедискаунтонкредитмемос</span><span class="sxs-lookup"><span data-stu-id="2d1ba-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="2d1ba-145">логический</span><span class="sxs-lookup"><span data-stu-id="2d1ba-145">boolean</span></span> |<span data-ttu-id="2d1ba-146">Указывает, следует ли применять скидку к кредитовым нотам.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="2d1ba-147">**Значение true** указывает, что будет задана скидка, **значение false** указывает, что скидка не будет задана.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="2d1ba-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d1ba-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="2d1ba-149">отличным</span><span class="sxs-lookup"><span data-stu-id="2d1ba-149">datetime</span></span>|<span data-ttu-id="2d1ba-150">Дата и время последнего изменения Пайменттермс.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="2d1ba-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="2d1ba-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="2d1ba-152">Relationships</span></span>
<span data-ttu-id="2d1ba-153">Нет</span><span class="sxs-lookup"><span data-stu-id="2d1ba-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d1ba-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d1ba-154">JSON representation</span></span>

<span data-ttu-id="2d1ba-155">Ниже показано представление объекта Пайменттермс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d1ba-155">Here is a JSON representation of the paymentTerms.</span></span>


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
