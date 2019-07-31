---
title: Тип ресурса Пайменттермс
description: Объект условий оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d367314d5546c59dd251b30e952aa17b9d60ce10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006600"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="989ad-103">Тип ресурса Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="989ad-103">paymentTerms resource type</span></span>
<span data-ttu-id="989ad-104">Представляет термин платежа в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="989ad-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="989ad-105">Методы</span><span class="sxs-lookup"><span data-stu-id="989ad-105">Methods</span></span>

| <span data-ttu-id="989ad-106">Метод</span><span class="sxs-lookup"><span data-stu-id="989ad-106">Method</span></span>                                                      | <span data-ttu-id="989ad-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="989ad-107">Return Type</span></span>|<span data-ttu-id="989ad-108">Описание</span><span class="sxs-lookup"><span data-stu-id="989ad-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="989ad-109">Получение Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="989ad-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="989ad-110">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="989ad-110">paymentTerms</span></span>|<span data-ttu-id="989ad-111">Получение объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="989ad-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="989ad-112">POST Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="989ad-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="989ad-113">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="989ad-113">paymentTerms</span></span>|<span data-ttu-id="989ad-114">Создайте объект формулы оплаты.</span><span class="sxs-lookup"><span data-stu-id="989ad-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="989ad-115">Исправление Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="989ad-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="989ad-116">Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="989ad-116">paymentTerms</span></span>|<span data-ttu-id="989ad-117">Обновление объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="989ad-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="989ad-118">Удаление Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="989ad-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="989ad-119">none</span><span class="sxs-lookup"><span data-stu-id="989ad-119">none</span></span>        |<span data-ttu-id="989ad-120">Удаление объекта условий оплаты.</span><span class="sxs-lookup"><span data-stu-id="989ad-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="989ad-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="989ad-121">Properties</span></span>
| <span data-ttu-id="989ad-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="989ad-122">Property</span></span>                     | <span data-ttu-id="989ad-123">Тип</span><span class="sxs-lookup"><span data-stu-id="989ad-123">Type</span></span>     |<span data-ttu-id="989ad-124">Описание</span><span class="sxs-lookup"><span data-stu-id="989ad-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="989ad-125">id</span><span class="sxs-lookup"><span data-stu-id="989ad-125">id</span></span>                            |<span data-ttu-id="989ad-126">GUID</span><span class="sxs-lookup"><span data-stu-id="989ad-126">GUID</span></span>    |<span data-ttu-id="989ad-127">Уникальный идентификатор Пайменттермс.</span><span class="sxs-lookup"><span data-stu-id="989ad-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="989ad-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="989ad-128">Non-editable.</span></span>           |
|<span data-ttu-id="989ad-129">code</span><span class="sxs-lookup"><span data-stu-id="989ad-129">code</span></span>                          |<span data-ttu-id="989ad-130">string</span><span class="sxs-lookup"><span data-stu-id="989ad-130">string</span></span>  |<span data-ttu-id="989ad-131">Определяет код условия платежа.</span><span class="sxs-lookup"><span data-stu-id="989ad-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="989ad-132">displayName</span><span class="sxs-lookup"><span data-stu-id="989ad-132">displayName</span></span>                   |<span data-ttu-id="989ad-133">string</span><span class="sxs-lookup"><span data-stu-id="989ad-133">string</span></span>  |<span data-ttu-id="989ad-134">Задает отображаемое имя условия платежа.</span><span class="sxs-lookup"><span data-stu-id="989ad-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="989ad-135">Дуедатекалкулатион</span><span class="sxs-lookup"><span data-stu-id="989ad-135">dueDateCalculation</span></span>            |<span data-ttu-id="989ad-136">string</span><span class="sxs-lookup"><span data-stu-id="989ad-136">string</span></span>  |<span data-ttu-id="989ad-137">Указывает формулу, используемую для расчета даты, на которую необходимо выполнить платеж.</span><span class="sxs-lookup"><span data-stu-id="989ad-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="989ad-138">Дискаунтдатекалкулатион</span><span class="sxs-lookup"><span data-stu-id="989ad-138">discountDateCalculation</span></span>       |<span data-ttu-id="989ad-139">string</span><span class="sxs-lookup"><span data-stu-id="989ad-139">string</span></span>  |<span data-ttu-id="989ad-140">Указывает формулу, используемую для расчета даты, которую необходимо выполнить для получения скидки.</span><span class="sxs-lookup"><span data-stu-id="989ad-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="989ad-141">Дискаунтперцент</span><span class="sxs-lookup"><span data-stu-id="989ad-141">discountPercent</span></span>               |<span data-ttu-id="989ad-142">числе</span><span class="sxs-lookup"><span data-stu-id="989ad-142">decimal</span></span> |<span data-ttu-id="989ad-143">Указывает процент скидки, который применяется для раннего платежа по сумме накладной.</span><span class="sxs-lookup"><span data-stu-id="989ad-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="989ad-144">Калкулатедискаунтонкредитмемос</span><span class="sxs-lookup"><span data-stu-id="989ad-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="989ad-145">boolean</span><span class="sxs-lookup"><span data-stu-id="989ad-145">boolean</span></span> |<span data-ttu-id="989ad-146">Указывает, следует ли применять скидку к кредитовым нотам.</span><span class="sxs-lookup"><span data-stu-id="989ad-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="989ad-147">**Значение true** указывает, что будет задана скидка, **значение false** указывает, что скидка не будет задана.</span><span class="sxs-lookup"><span data-stu-id="989ad-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="989ad-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="989ad-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="989ad-149">отличным</span><span class="sxs-lookup"><span data-stu-id="989ad-149">datetime</span></span>|<span data-ttu-id="989ad-150">Дата и время последнего изменения Пайменттермс.</span><span class="sxs-lookup"><span data-stu-id="989ad-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="989ad-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="989ad-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="989ad-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="989ad-152">Relationships</span></span>
<span data-ttu-id="989ad-153">Нет</span><span class="sxs-lookup"><span data-stu-id="989ad-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="989ad-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="989ad-154">JSON representation</span></span>

<span data-ttu-id="989ad-155">Ниже показано представление объекта Пайменттермс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="989ad-155">Here is a JSON representation of the paymentTerms.</span></span>


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
