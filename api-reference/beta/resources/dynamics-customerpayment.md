---
title: Тип ресурса Кустомерпайментс
description: Объект платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9063a9066c51956596e4f0aa918a2e7a53bf2ab9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365614"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="e18b3-103">Тип ресурса Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="e18b3-103">customerPayments resource type</span></span>
<span data-ttu-id="e18b3-104">Представляет платеж клиента в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="e18b3-104">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="e18b3-105">Клиентская оплата вводится в виде строки в журнале платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-105">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="e18b3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e18b3-106">Methods</span></span>

| <span data-ttu-id="e18b3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e18b3-107">Method</span></span>         | <span data-ttu-id="e18b3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e18b3-108">Return Type</span></span>  |<span data-ttu-id="e18b3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e18b3-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="e18b3-110">Получение Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="e18b3-110">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="e18b3-111">Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="e18b3-111">customerPayments</span></span>|<span data-ttu-id="e18b3-112">Возвращает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-112">Gets a customer payment.</span></span>|
|[<span data-ttu-id="e18b3-113">POST Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="e18b3-113">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="e18b3-114">Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="e18b3-114">customerPayments</span></span>|<span data-ttu-id="e18b3-115">Создает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-115">Creates a customer payment.</span></span>|
|[<span data-ttu-id="e18b3-116">Исправление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="e18b3-116">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="e18b3-117">Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="e18b3-117">customerPayments</span></span>|<span data-ttu-id="e18b3-118">Обновляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-118">Updates a customer payment.</span></span>|
|[<span data-ttu-id="e18b3-119">Удаление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="e18b3-119">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="e18b3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e18b3-120">none</span></span>|<span data-ttu-id="e18b3-121">Удаляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-121">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="e18b3-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="e18b3-122">Properties</span></span>
| <span data-ttu-id="e18b3-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="e18b3-123">Property</span></span>     | <span data-ttu-id="e18b3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e18b3-124">Type</span></span>    |<span data-ttu-id="e18b3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e18b3-125">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="e18b3-126">id</span><span class="sxs-lookup"><span data-stu-id="e18b3-126">id</span></span>|<span data-ttu-id="e18b3-127">GUID</span><span class="sxs-lookup"><span data-stu-id="e18b3-127">GUID</span></span>|<span data-ttu-id="e18b3-128">Уникальный идентификатор платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-128">The unique ID of the customer payment.</span></span> <span data-ttu-id="e18b3-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="e18b3-129">Non-editable.</span></span>|
|<span data-ttu-id="e18b3-130">Жаурналдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="e18b3-130">journalDisplayName</span></span>|<span data-ttu-id="e18b3-131">строка</span><span class="sxs-lookup"><span data-stu-id="e18b3-131">string</span></span>|<span data-ttu-id="e18b3-132">Журнал платежей клиента, в котором запись платежа является строкой.</span><span class="sxs-lookup"><span data-stu-id="e18b3-132">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="e18b3-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="e18b3-133">lineNumber</span></span>|<span data-ttu-id="e18b3-134">целое число</span><span class="sxs-lookup"><span data-stu-id="e18b3-134">integer</span></span>|<span data-ttu-id="e18b3-135">Номер платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-135">The number of the customer payment.</span></span>|
|<span data-ttu-id="e18b3-136">customerId</span><span class="sxs-lookup"><span data-stu-id="e18b3-136">customerId</span></span>|<span data-ttu-id="e18b3-137">GUID</span><span class="sxs-lookup"><span data-stu-id="e18b3-137">GUID</span></span>|<span data-ttu-id="e18b3-138">Уникальный идентификатор клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="e18b3-138">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="e18b3-139">Кустомернумбер</span><span class="sxs-lookup"><span data-stu-id="e18b3-139">customerNumber</span></span>|<span data-ttu-id="e18b3-140">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="e18b3-140">string, maximum size 20</span></span>|<span data-ttu-id="e18b3-141">Номер клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="e18b3-141">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="e18b3-142">contactId</span><span class="sxs-lookup"><span data-stu-id="e18b3-142">contactId</span></span>|<span data-ttu-id="e18b3-143">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="e18b3-143">string, maximum size 250</span></span>|<span data-ttu-id="e18b3-144">Идентификатор контакта Exchange для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-144">The exchange contact id for the given customer.</span></span> <span data-ttu-id="e18b3-145">Если идентификатор клиента не указан, мы будем использовать идентификатор контакта, чтобы найти его.</span><span class="sxs-lookup"><span data-stu-id="e18b3-145">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="e18b3-146">Постингдате</span><span class="sxs-lookup"><span data-stu-id="e18b3-146">postingDate</span></span>|<span data-ttu-id="e18b3-147">дата</span><span class="sxs-lookup"><span data-stu-id="e18b3-147">date</span></span>|<span data-ttu-id="e18b3-148">Дата, когда выполняется разноска платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-148">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="e18b3-149">Документнумбер</span><span class="sxs-lookup"><span data-stu-id="e18b3-149">documentNumber</span></span>|<span data-ttu-id="e18b3-150">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="e18b3-150">string, maximum size 20</span></span>|<span data-ttu-id="e18b3-151">Указывает номер документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-151">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="e18b3-152">Екстерналдокументнумбер</span><span class="sxs-lookup"><span data-stu-id="e18b3-152">externalDocumentNumber</span></span>|<span data-ttu-id="e18b3-153">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="e18b3-153">string, maximum size 20</span></span>|<span data-ttu-id="e18b3-154">Указывает номер внешнего документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-154">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="e18b3-155">отступ</span><span class="sxs-lookup"><span data-stu-id="e18b3-155">amount</span></span>|<span data-ttu-id="e18b3-156">числе</span><span class="sxs-lookup"><span data-stu-id="e18b3-156">decimal</span></span>|<span data-ttu-id="e18b3-157">Указывает общую сумму (включая НДС), из которой состоит платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-157">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="e18b3-158">Апплиестоинвоицеид</span><span class="sxs-lookup"><span data-stu-id="e18b3-158">appliesToInvoiceId</span></span>|<span data-ttu-id="e18b3-159">GUID</span><span class="sxs-lookup"><span data-stu-id="e18b3-159">GUID</span></span>|<span data-ttu-id="e18b3-160">Уникальный идентификатор счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="e18b3-160">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="e18b3-161">Апплиестоинвоиценумбер</span><span class="sxs-lookup"><span data-stu-id="e18b3-161">appliesToInvoiceNumber</span></span>|<span data-ttu-id="e18b3-162">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="e18b3-162">string, maximum size 20</span></span>|<span data-ttu-id="e18b3-163">Номер счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="e18b3-163">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="e18b3-164">description</span><span class="sxs-lookup"><span data-stu-id="e18b3-164">description</span></span>|<span data-ttu-id="e18b3-165">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="e18b3-165">string, maximum size 50</span></span>|<span data-ttu-id="e18b3-166">Описание платежа клиента, предоставленное пользователем или созданным пользователем.</span><span class="sxs-lookup"><span data-stu-id="e18b3-166">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="e18b3-167">комментарий</span><span class="sxs-lookup"><span data-stu-id="e18b3-167">comment</span></span>|<span data-ttu-id="e18b3-168">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="e18b3-168">string, maximum size 250</span></span>|<span data-ttu-id="e18b3-169">Указанный пользователем комментарий к платежу клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-169">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="e18b3-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e18b3-170">lastModifiedDateTime</span></span>|<span data-ttu-id="e18b3-171">отличным</span><span class="sxs-lookup"><span data-stu-id="e18b3-171">datetime</span></span>|<span data-ttu-id="e18b3-172">Дата и время последнего изменения платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-172">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="e18b3-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e18b3-173">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e18b3-174">Отношения</span><span class="sxs-lookup"><span data-stu-id="e18b3-174">Relationships</span></span>
<span data-ttu-id="e18b3-175">Платеж клиента — это вложенная страница журнала платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="e18b3-175">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="e18b3-176">Прямой доступ к нему невозможен.</span><span class="sxs-lookup"><span data-stu-id="e18b3-176">It cannot be accessed directly.</span></span>

<span data-ttu-id="e18b3-177">Платеж клиента может быть "родительским объектом" строк измерения.</span><span class="sxs-lookup"><span data-stu-id="e18b3-177">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="e18b3-178">Клиент (customerId) должен существовать в таблице Customers (клиенты).</span><span class="sxs-lookup"><span data-stu-id="e18b3-178">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="e18b3-179">Счет (Апплиестоинвоицеид) должен существовать в таблице "счета продаж".</span><span class="sxs-lookup"><span data-stu-id="e18b3-179">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e18b3-180">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e18b3-180">JSON representation</span></span>

<span data-ttu-id="e18b3-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e18b3-181">Here is a JSON representation of the resource.</span></span>

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

