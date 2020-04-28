---
title: Тип ресурса Кустомерпайментс
description: Объект платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bd990ea9778ada7d43c9b8192d77cf8af618909b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504638"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="a6103-103">Тип ресурса Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="a6103-103">customerPayments resource type</span></span>

<span data-ttu-id="a6103-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6103-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6103-105">Представляет платеж клиента в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a6103-105">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="a6103-106">Клиентская оплата вводится в виде строки в журнале платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-106">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="a6103-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a6103-107">Methods</span></span>

| <span data-ttu-id="a6103-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a6103-108">Method</span></span>         | <span data-ttu-id="a6103-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a6103-109">Return Type</span></span>  |<span data-ttu-id="a6103-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a6103-110">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="a6103-111">Получение Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="a6103-111">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="a6103-112">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="a6103-112">customerPayments</span></span>|<span data-ttu-id="a6103-113">Возвращает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-113">Gets a customer payment.</span></span>|
|[<span data-ttu-id="a6103-114">POST Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="a6103-114">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="a6103-115">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="a6103-115">customerPayments</span></span>|<span data-ttu-id="a6103-116">Создает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-116">Creates a customer payment.</span></span>|
|[<span data-ttu-id="a6103-117">Исправление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="a6103-117">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="a6103-118">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="a6103-118">customerPayments</span></span>|<span data-ttu-id="a6103-119">Обновляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-119">Updates a customer payment.</span></span>|
|[<span data-ttu-id="a6103-120">Удаление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="a6103-120">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="a6103-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a6103-121">none</span></span>|<span data-ttu-id="a6103-122">Удаляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-122">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6103-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6103-123">Properties</span></span>
| <span data-ttu-id="a6103-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6103-124">Property</span></span>     | <span data-ttu-id="a6103-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a6103-125">Type</span></span>    |<span data-ttu-id="a6103-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a6103-126">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="a6103-127">id</span><span class="sxs-lookup"><span data-stu-id="a6103-127">id</span></span>|<span data-ttu-id="a6103-128">GUID</span><span class="sxs-lookup"><span data-stu-id="a6103-128">GUID</span></span>|<span data-ttu-id="a6103-129">Уникальный идентификатор платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-129">The unique ID of the customer payment.</span></span> <span data-ttu-id="a6103-130">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="a6103-130">Non-editable.</span></span>|
|<span data-ttu-id="a6103-131">жаурналдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="a6103-131">journalDisplayName</span></span>|<span data-ttu-id="a6103-132">string</span><span class="sxs-lookup"><span data-stu-id="a6103-132">string</span></span>|<span data-ttu-id="a6103-133">Журнал платежей клиента, в котором запись платежа является строкой.</span><span class="sxs-lookup"><span data-stu-id="a6103-133">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="a6103-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="a6103-134">lineNumber</span></span>|<span data-ttu-id="a6103-135">целое</span><span class="sxs-lookup"><span data-stu-id="a6103-135">integer</span></span>|<span data-ttu-id="a6103-136">Номер платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-136">The number of the customer payment.</span></span>|
|<span data-ttu-id="a6103-137">customerId</span><span class="sxs-lookup"><span data-stu-id="a6103-137">customerId</span></span>|<span data-ttu-id="a6103-138">GUID</span><span class="sxs-lookup"><span data-stu-id="a6103-138">GUID</span></span>|<span data-ttu-id="a6103-139">Уникальный идентификатор клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="a6103-139">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="a6103-140">кустомернумбер</span><span class="sxs-lookup"><span data-stu-id="a6103-140">customerNumber</span></span>|<span data-ttu-id="a6103-141">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="a6103-141">string, maximum size 20</span></span>|<span data-ttu-id="a6103-142">Номер клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="a6103-142">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="a6103-143">contactId</span><span class="sxs-lookup"><span data-stu-id="a6103-143">contactId</span></span>|<span data-ttu-id="a6103-144">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="a6103-144">string, maximum size 250</span></span>|<span data-ttu-id="a6103-145">Идентификатор контакта Exchange для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-145">The exchange contact id for the given customer.</span></span> <span data-ttu-id="a6103-146">Если идентификатор клиента не указан, мы будем использовать идентификатор контакта, чтобы найти его.</span><span class="sxs-lookup"><span data-stu-id="a6103-146">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="a6103-147">постингдате</span><span class="sxs-lookup"><span data-stu-id="a6103-147">postingDate</span></span>|<span data-ttu-id="a6103-148">date</span><span class="sxs-lookup"><span data-stu-id="a6103-148">date</span></span>|<span data-ttu-id="a6103-149">Дата, когда выполняется разноска платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-149">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="a6103-150">документнумбер</span><span class="sxs-lookup"><span data-stu-id="a6103-150">documentNumber</span></span>|<span data-ttu-id="a6103-151">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="a6103-151">string, maximum size 20</span></span>|<span data-ttu-id="a6103-152">Указывает номер документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-152">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="a6103-153">екстерналдокументнумбер</span><span class="sxs-lookup"><span data-stu-id="a6103-153">externalDocumentNumber</span></span>|<span data-ttu-id="a6103-154">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="a6103-154">string, maximum size 20</span></span>|<span data-ttu-id="a6103-155">Указывает номер внешнего документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-155">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="a6103-156">отступ</span><span class="sxs-lookup"><span data-stu-id="a6103-156">amount</span></span>|<span data-ttu-id="a6103-157">числе</span><span class="sxs-lookup"><span data-stu-id="a6103-157">decimal</span></span>|<span data-ttu-id="a6103-158">Указывает общую сумму (включая НДС), из которой состоит платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-158">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="a6103-159">апплиестоинвоицеид</span><span class="sxs-lookup"><span data-stu-id="a6103-159">appliesToInvoiceId</span></span>|<span data-ttu-id="a6103-160">GUID</span><span class="sxs-lookup"><span data-stu-id="a6103-160">GUID</span></span>|<span data-ttu-id="a6103-161">Уникальный идентификатор счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="a6103-161">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="a6103-162">апплиестоинвоиценумбер</span><span class="sxs-lookup"><span data-stu-id="a6103-162">appliesToInvoiceNumber</span></span>|<span data-ttu-id="a6103-163">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="a6103-163">string, maximum size 20</span></span>|<span data-ttu-id="a6103-164">Номер счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="a6103-164">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="a6103-165">description</span><span class="sxs-lookup"><span data-stu-id="a6103-165">description</span></span>|<span data-ttu-id="a6103-166">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="a6103-166">string, maximum size 50</span></span>|<span data-ttu-id="a6103-167">Описание платежа клиента, предоставленное пользователем или созданным пользователем.</span><span class="sxs-lookup"><span data-stu-id="a6103-167">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="a6103-168">comment</span><span class="sxs-lookup"><span data-stu-id="a6103-168">comment</span></span>|<span data-ttu-id="a6103-169">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="a6103-169">string, maximum size 250</span></span>|<span data-ttu-id="a6103-170">Указанный пользователем комментарий к платежу клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-170">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="a6103-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6103-171">lastModifiedDateTime</span></span>|<span data-ttu-id="a6103-172">datetime</span><span class="sxs-lookup"><span data-stu-id="a6103-172">datetime</span></span>|<span data-ttu-id="a6103-173">Дата и время последнего изменения платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-173">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="a6103-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6103-174">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a6103-175">Связи</span><span class="sxs-lookup"><span data-stu-id="a6103-175">Relationships</span></span>
<span data-ttu-id="a6103-176">Платеж клиента — это вложенная страница журнала платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="a6103-176">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="a6103-177">Прямой доступ к нему невозможен.</span><span class="sxs-lookup"><span data-stu-id="a6103-177">It cannot be accessed directly.</span></span>

<span data-ttu-id="a6103-178">Платеж клиента может быть "родительским объектом" строк измерения.</span><span class="sxs-lookup"><span data-stu-id="a6103-178">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="a6103-179">Клиент (customerId) должен существовать в таблице Customers (клиенты).</span><span class="sxs-lookup"><span data-stu-id="a6103-179">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="a6103-180">Счет (Апплиестоинвоицеид) должен существовать в таблице "счета продаж".</span><span class="sxs-lookup"><span data-stu-id="a6103-180">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a6103-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6103-181">JSON representation</span></span>

<span data-ttu-id="a6103-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6103-182">Here is a JSON representation of the resource.</span></span>

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

