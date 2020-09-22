---
title: Тип ресурса Кустомерпайментс
description: Объект платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bf5536181f965765615a7e2d707d6503813cfb76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040051"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="95e31-103">Тип ресурса Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="95e31-103">customerPayments resource type</span></span>

<span data-ttu-id="95e31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95e31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95e31-105">Представляет платеж клиента в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="95e31-105">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="95e31-106">Клиентская оплата вводится в виде строки в журнале платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-106">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="95e31-107">Методы</span><span class="sxs-lookup"><span data-stu-id="95e31-107">Methods</span></span>

| <span data-ttu-id="95e31-108">Метод</span><span class="sxs-lookup"><span data-stu-id="95e31-108">Method</span></span>         | <span data-ttu-id="95e31-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95e31-109">Return Type</span></span>  |<span data-ttu-id="95e31-110">Описание</span><span class="sxs-lookup"><span data-stu-id="95e31-110">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="95e31-111">Получение Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="95e31-111">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="95e31-112">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="95e31-112">customerPayments</span></span>|<span data-ttu-id="95e31-113">Возвращает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-113">Gets a customer payment.</span></span>|
|[<span data-ttu-id="95e31-114">POST Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="95e31-114">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="95e31-115">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="95e31-115">customerPayments</span></span>|<span data-ttu-id="95e31-116">Создает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-116">Creates a customer payment.</span></span>|
|[<span data-ttu-id="95e31-117">Исправление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="95e31-117">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="95e31-118">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="95e31-118">customerPayments</span></span>|<span data-ttu-id="95e31-119">Обновляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-119">Updates a customer payment.</span></span>|
|[<span data-ttu-id="95e31-120">Удаление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="95e31-120">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="95e31-121">Нет</span><span class="sxs-lookup"><span data-stu-id="95e31-121">none</span></span>|<span data-ttu-id="95e31-122">Удаляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-122">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="95e31-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="95e31-123">Properties</span></span>
| <span data-ttu-id="95e31-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="95e31-124">Property</span></span>     | <span data-ttu-id="95e31-125">Тип</span><span class="sxs-lookup"><span data-stu-id="95e31-125">Type</span></span>    |<span data-ttu-id="95e31-126">Описание</span><span class="sxs-lookup"><span data-stu-id="95e31-126">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="95e31-127">id</span><span class="sxs-lookup"><span data-stu-id="95e31-127">id</span></span>|<span data-ttu-id="95e31-128">GUID</span><span class="sxs-lookup"><span data-stu-id="95e31-128">GUID</span></span>|<span data-ttu-id="95e31-129">Уникальный идентификатор платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-129">The unique ID of the customer payment.</span></span> <span data-ttu-id="95e31-130">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="95e31-130">Non-editable.</span></span>|
|<span data-ttu-id="95e31-131">жаурналдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="95e31-131">journalDisplayName</span></span>|<span data-ttu-id="95e31-132">string</span><span class="sxs-lookup"><span data-stu-id="95e31-132">string</span></span>|<span data-ttu-id="95e31-133">Журнал платежей клиента, в котором запись платежа является строкой.</span><span class="sxs-lookup"><span data-stu-id="95e31-133">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="95e31-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="95e31-134">lineNumber</span></span>|<span data-ttu-id="95e31-135">целое</span><span class="sxs-lookup"><span data-stu-id="95e31-135">integer</span></span>|<span data-ttu-id="95e31-136">Номер платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-136">The number of the customer payment.</span></span>|
|<span data-ttu-id="95e31-137">customerId</span><span class="sxs-lookup"><span data-stu-id="95e31-137">customerId</span></span>|<span data-ttu-id="95e31-138">GUID</span><span class="sxs-lookup"><span data-stu-id="95e31-138">GUID</span></span>|<span data-ttu-id="95e31-139">Уникальный идентификатор клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="95e31-139">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="95e31-140">кустомернумбер</span><span class="sxs-lookup"><span data-stu-id="95e31-140">customerNumber</span></span>|<span data-ttu-id="95e31-141">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="95e31-141">string, maximum size 20</span></span>|<span data-ttu-id="95e31-142">Номер клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="95e31-142">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="95e31-143">contactId</span><span class="sxs-lookup"><span data-stu-id="95e31-143">contactId</span></span>|<span data-ttu-id="95e31-144">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="95e31-144">string, maximum size 250</span></span>|<span data-ttu-id="95e31-145">Идентификатор контакта Exchange для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-145">The exchange contact id for the given customer.</span></span> <span data-ttu-id="95e31-146">Если идентификатор клиента не указан, мы будем использовать идентификатор контакта, чтобы найти его.</span><span class="sxs-lookup"><span data-stu-id="95e31-146">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="95e31-147">постингдате</span><span class="sxs-lookup"><span data-stu-id="95e31-147">postingDate</span></span>|<span data-ttu-id="95e31-148">date</span><span class="sxs-lookup"><span data-stu-id="95e31-148">date</span></span>|<span data-ttu-id="95e31-149">Дата, когда выполняется разноска платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-149">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="95e31-150">документнумбер</span><span class="sxs-lookup"><span data-stu-id="95e31-150">documentNumber</span></span>|<span data-ttu-id="95e31-151">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="95e31-151">string, maximum size 20</span></span>|<span data-ttu-id="95e31-152">Указывает номер документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-152">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="95e31-153">екстерналдокументнумбер</span><span class="sxs-lookup"><span data-stu-id="95e31-153">externalDocumentNumber</span></span>|<span data-ttu-id="95e31-154">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="95e31-154">string, maximum size 20</span></span>|<span data-ttu-id="95e31-155">Указывает номер внешнего документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-155">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="95e31-156">отступ</span><span class="sxs-lookup"><span data-stu-id="95e31-156">amount</span></span>|<span data-ttu-id="95e31-157">числе</span><span class="sxs-lookup"><span data-stu-id="95e31-157">decimal</span></span>|<span data-ttu-id="95e31-158">Указывает общую сумму (включая НДС), из которой состоит платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-158">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="95e31-159">апплиестоинвоицеид</span><span class="sxs-lookup"><span data-stu-id="95e31-159">appliesToInvoiceId</span></span>|<span data-ttu-id="95e31-160">GUID</span><span class="sxs-lookup"><span data-stu-id="95e31-160">GUID</span></span>|<span data-ttu-id="95e31-161">Уникальный идентификатор счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="95e31-161">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="95e31-162">апплиестоинвоиценумбер</span><span class="sxs-lookup"><span data-stu-id="95e31-162">appliesToInvoiceNumber</span></span>|<span data-ttu-id="95e31-163">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="95e31-163">string, maximum size 20</span></span>|<span data-ttu-id="95e31-164">Номер счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="95e31-164">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="95e31-165">description</span><span class="sxs-lookup"><span data-stu-id="95e31-165">description</span></span>|<span data-ttu-id="95e31-166">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="95e31-166">string, maximum size 50</span></span>|<span data-ttu-id="95e31-167">Описание платежа клиента, предоставленное пользователем или созданным пользователем.</span><span class="sxs-lookup"><span data-stu-id="95e31-167">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="95e31-168">comment</span><span class="sxs-lookup"><span data-stu-id="95e31-168">comment</span></span>|<span data-ttu-id="95e31-169">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="95e31-169">string, maximum size 250</span></span>|<span data-ttu-id="95e31-170">Указанный пользователем комментарий к платежу клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-170">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="95e31-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95e31-171">lastModifiedDateTime</span></span>|<span data-ttu-id="95e31-172">datetime</span><span class="sxs-lookup"><span data-stu-id="95e31-172">datetime</span></span>|<span data-ttu-id="95e31-173">Дата и время последнего изменения платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-173">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="95e31-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95e31-174">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="95e31-175">Связи</span><span class="sxs-lookup"><span data-stu-id="95e31-175">Relationships</span></span>
<span data-ttu-id="95e31-176">Платеж клиента — это вложенная страница журнала платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="95e31-176">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="95e31-177">Прямой доступ к нему невозможен.</span><span class="sxs-lookup"><span data-stu-id="95e31-177">It cannot be accessed directly.</span></span>

<span data-ttu-id="95e31-178">Платеж клиента может быть "родительским объектом" строк измерения.</span><span class="sxs-lookup"><span data-stu-id="95e31-178">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="95e31-179">Клиент (customerId) должен существовать в таблице Customers (клиенты).</span><span class="sxs-lookup"><span data-stu-id="95e31-179">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="95e31-180">Счет (Апплиестоинвоицеид) должен существовать в таблице "счета продаж".</span><span class="sxs-lookup"><span data-stu-id="95e31-180">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="95e31-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95e31-181">JSON representation</span></span>

<span data-ttu-id="95e31-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95e31-182">Here is a JSON representation of the resource.</span></span>

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



