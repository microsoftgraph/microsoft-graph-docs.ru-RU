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
# <a name="customerpayments-resource-type"></a><span data-ttu-id="b050c-103">Тип ресурса Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="b050c-103">customerPayments resource type</span></span>

<span data-ttu-id="b050c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b050c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b050c-105">Представляет платеж клиента в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b050c-105">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="b050c-106">Клиентская оплата вводится в виде строки в журнале платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-106">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="b050c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b050c-107">Methods</span></span>

| <span data-ttu-id="b050c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b050c-108">Method</span></span>         | <span data-ttu-id="b050c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b050c-109">Return Type</span></span>  |<span data-ttu-id="b050c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b050c-110">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="b050c-111">Получение Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="b050c-111">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="b050c-112">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="b050c-112">customerPayments</span></span>|<span data-ttu-id="b050c-113">Возвращает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-113">Gets a customer payment.</span></span>|
|[<span data-ttu-id="b050c-114">POST Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="b050c-114">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="b050c-115">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="b050c-115">customerPayments</span></span>|<span data-ttu-id="b050c-116">Создает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-116">Creates a customer payment.</span></span>|
|[<span data-ttu-id="b050c-117">Исправление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="b050c-117">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="b050c-118">кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="b050c-118">customerPayments</span></span>|<span data-ttu-id="b050c-119">Обновляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-119">Updates a customer payment.</span></span>|
|[<span data-ttu-id="b050c-120">Удаление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="b050c-120">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="b050c-121">нет</span><span class="sxs-lookup"><span data-stu-id="b050c-121">none</span></span>|<span data-ttu-id="b050c-122">Удаляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-122">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="b050c-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="b050c-123">Properties</span></span>
| <span data-ttu-id="b050c-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="b050c-124">Property</span></span>     | <span data-ttu-id="b050c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b050c-125">Type</span></span>    |<span data-ttu-id="b050c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b050c-126">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="b050c-127">id</span><span class="sxs-lookup"><span data-stu-id="b050c-127">id</span></span>|<span data-ttu-id="b050c-128">GUID</span><span class="sxs-lookup"><span data-stu-id="b050c-128">GUID</span></span>|<span data-ttu-id="b050c-129">Уникальный идентификатор платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-129">The unique ID of the customer payment.</span></span> <span data-ttu-id="b050c-130">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="b050c-130">Non-editable.</span></span>|
|<span data-ttu-id="b050c-131">жаурналдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="b050c-131">journalDisplayName</span></span>|<span data-ttu-id="b050c-132">строка</span><span class="sxs-lookup"><span data-stu-id="b050c-132">string</span></span>|<span data-ttu-id="b050c-133">Журнал платежей клиента, в котором запись платежа является строкой.</span><span class="sxs-lookup"><span data-stu-id="b050c-133">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="b050c-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="b050c-134">lineNumber</span></span>|<span data-ttu-id="b050c-135">целое</span><span class="sxs-lookup"><span data-stu-id="b050c-135">integer</span></span>|<span data-ttu-id="b050c-136">Номер платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-136">The number of the customer payment.</span></span>|
|<span data-ttu-id="b050c-137">customerId</span><span class="sxs-lookup"><span data-stu-id="b050c-137">customerId</span></span>|<span data-ttu-id="b050c-138">GUID</span><span class="sxs-lookup"><span data-stu-id="b050c-138">GUID</span></span>|<span data-ttu-id="b050c-139">Уникальный идентификатор клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="b050c-139">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="b050c-140">кустомернумбер</span><span class="sxs-lookup"><span data-stu-id="b050c-140">customerNumber</span></span>|<span data-ttu-id="b050c-141">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="b050c-141">string, maximum size 20</span></span>|<span data-ttu-id="b050c-142">Номер клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="b050c-142">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="b050c-143">contactId</span><span class="sxs-lookup"><span data-stu-id="b050c-143">contactId</span></span>|<span data-ttu-id="b050c-144">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="b050c-144">string, maximum size 250</span></span>|<span data-ttu-id="b050c-145">Идентификатор контакта Exchange для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-145">The exchange contact id for the given customer.</span></span> <span data-ttu-id="b050c-146">Если идентификатор клиента не указан, мы будем использовать идентификатор контакта, чтобы найти его.</span><span class="sxs-lookup"><span data-stu-id="b050c-146">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="b050c-147">постингдате</span><span class="sxs-lookup"><span data-stu-id="b050c-147">postingDate</span></span>|<span data-ttu-id="b050c-148">date</span><span class="sxs-lookup"><span data-stu-id="b050c-148">date</span></span>|<span data-ttu-id="b050c-149">Дата, когда выполняется разноска платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-149">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="b050c-150">документнумбер</span><span class="sxs-lookup"><span data-stu-id="b050c-150">documentNumber</span></span>|<span data-ttu-id="b050c-151">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="b050c-151">string, maximum size 20</span></span>|<span data-ttu-id="b050c-152">Указывает номер документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-152">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="b050c-153">екстерналдокументнумбер</span><span class="sxs-lookup"><span data-stu-id="b050c-153">externalDocumentNumber</span></span>|<span data-ttu-id="b050c-154">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="b050c-154">string, maximum size 20</span></span>|<span data-ttu-id="b050c-155">Указывает номер внешнего документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-155">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="b050c-156">отступ</span><span class="sxs-lookup"><span data-stu-id="b050c-156">amount</span></span>|<span data-ttu-id="b050c-157">числе</span><span class="sxs-lookup"><span data-stu-id="b050c-157">decimal</span></span>|<span data-ttu-id="b050c-158">Указывает общую сумму (включая НДС), из которой состоит платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-158">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="b050c-159">апплиестоинвоицеид</span><span class="sxs-lookup"><span data-stu-id="b050c-159">appliesToInvoiceId</span></span>|<span data-ttu-id="b050c-160">GUID</span><span class="sxs-lookup"><span data-stu-id="b050c-160">GUID</span></span>|<span data-ttu-id="b050c-161">Уникальный идентификатор счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="b050c-161">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="b050c-162">апплиестоинвоиценумбер</span><span class="sxs-lookup"><span data-stu-id="b050c-162">appliesToInvoiceNumber</span></span>|<span data-ttu-id="b050c-163">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="b050c-163">string, maximum size 20</span></span>|<span data-ttu-id="b050c-164">Номер счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="b050c-164">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="b050c-165">description</span><span class="sxs-lookup"><span data-stu-id="b050c-165">description</span></span>|<span data-ttu-id="b050c-166">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="b050c-166">string, maximum size 50</span></span>|<span data-ttu-id="b050c-167">Описание платежа клиента, предоставленное пользователем или созданным пользователем.</span><span class="sxs-lookup"><span data-stu-id="b050c-167">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="b050c-168">comment</span><span class="sxs-lookup"><span data-stu-id="b050c-168">comment</span></span>|<span data-ttu-id="b050c-169">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="b050c-169">string, maximum size 250</span></span>|<span data-ttu-id="b050c-170">Указанный пользователем комментарий к платежу клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-170">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="b050c-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b050c-171">lastModifiedDateTime</span></span>|<span data-ttu-id="b050c-172">datetime</span><span class="sxs-lookup"><span data-stu-id="b050c-172">datetime</span></span>|<span data-ttu-id="b050c-173">Дата и время последнего изменения платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-173">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="b050c-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b050c-174">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b050c-175">Связи</span><span class="sxs-lookup"><span data-stu-id="b050c-175">Relationships</span></span>
<span data-ttu-id="b050c-176">Платеж клиента — это вложенная страница журнала платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="b050c-176">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="b050c-177">Прямой доступ к нему невозможен.</span><span class="sxs-lookup"><span data-stu-id="b050c-177">It cannot be accessed directly.</span></span>

<span data-ttu-id="b050c-178">Платеж клиента может быть "родительским объектом" строк измерения.</span><span class="sxs-lookup"><span data-stu-id="b050c-178">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="b050c-179">Клиент (customerId) должен существовать в таблице Customers (клиенты).</span><span class="sxs-lookup"><span data-stu-id="b050c-179">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="b050c-180">Счет (Апплиестоинвоицеид) должен существовать в таблице "счета продаж".</span><span class="sxs-lookup"><span data-stu-id="b050c-180">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b050c-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b050c-181">JSON representation</span></span>

<span data-ttu-id="b050c-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b050c-182">Here is a JSON representation of the resource.</span></span>

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

