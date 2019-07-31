---
title: Тип ресурса Кустомерпайментс
description: Объект платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 4a1c777d51dd1ba706af85f431162cda16b5d25b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012606"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="52647-103">Тип ресурса Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="52647-103">customerPayments resource type</span></span>
<span data-ttu-id="52647-104">Представляет платеж клиента в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="52647-104">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="52647-105">Клиентская оплата вводится в виде строки в журнале платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-105">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="52647-106">Методы</span><span class="sxs-lookup"><span data-stu-id="52647-106">Methods</span></span>

| <span data-ttu-id="52647-107">Метод</span><span class="sxs-lookup"><span data-stu-id="52647-107">Method</span></span>         | <span data-ttu-id="52647-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52647-108">Return Type</span></span>  |<span data-ttu-id="52647-109">Описание</span><span class="sxs-lookup"><span data-stu-id="52647-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="52647-110">Получение Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="52647-110">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="52647-111">Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="52647-111">customerPayments</span></span>|<span data-ttu-id="52647-112">Возвращает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-112">Gets a customer payment.</span></span>|
|[<span data-ttu-id="52647-113">POST Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="52647-113">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="52647-114">Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="52647-114">customerPayments</span></span>|<span data-ttu-id="52647-115">Создает платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-115">Creates a customer payment.</span></span>|
|[<span data-ttu-id="52647-116">Исправление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="52647-116">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="52647-117">Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="52647-117">customerPayments</span></span>|<span data-ttu-id="52647-118">Обновляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-118">Updates a customer payment.</span></span>|
|[<span data-ttu-id="52647-119">Удаление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="52647-119">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="52647-120">none</span><span class="sxs-lookup"><span data-stu-id="52647-120">none</span></span>|<span data-ttu-id="52647-121">Удаляет платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-121">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="52647-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="52647-122">Properties</span></span>
| <span data-ttu-id="52647-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="52647-123">Property</span></span>     | <span data-ttu-id="52647-124">Тип</span><span class="sxs-lookup"><span data-stu-id="52647-124">Type</span></span>    |<span data-ttu-id="52647-125">Описание</span><span class="sxs-lookup"><span data-stu-id="52647-125">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="52647-126">id</span><span class="sxs-lookup"><span data-stu-id="52647-126">id</span></span>|<span data-ttu-id="52647-127">GUID</span><span class="sxs-lookup"><span data-stu-id="52647-127">GUID</span></span>|<span data-ttu-id="52647-128">Уникальный идентификатор платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-128">The unique ID of the customer payment.</span></span> <span data-ttu-id="52647-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="52647-129">Non-editable.</span></span>|
|<span data-ttu-id="52647-130">Жаурналдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="52647-130">journalDisplayName</span></span>|<span data-ttu-id="52647-131">string</span><span class="sxs-lookup"><span data-stu-id="52647-131">string</span></span>|<span data-ttu-id="52647-132">Журнал платежей клиента, в котором запись платежа является строкой.</span><span class="sxs-lookup"><span data-stu-id="52647-132">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="52647-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="52647-133">lineNumber</span></span>|<span data-ttu-id="52647-134">целое</span><span class="sxs-lookup"><span data-stu-id="52647-134">integer</span></span>|<span data-ttu-id="52647-135">Номер платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-135">The number of the customer payment.</span></span>|
|<span data-ttu-id="52647-136">customerId</span><span class="sxs-lookup"><span data-stu-id="52647-136">customerId</span></span>|<span data-ttu-id="52647-137">GUID</span><span class="sxs-lookup"><span data-stu-id="52647-137">GUID</span></span>|<span data-ttu-id="52647-138">Уникальный идентификатор клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="52647-138">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="52647-139">Кустомернумбер</span><span class="sxs-lookup"><span data-stu-id="52647-139">customerNumber</span></span>|<span data-ttu-id="52647-140">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="52647-140">string, maximum size 20</span></span>|<span data-ttu-id="52647-141">Номер клиента, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="52647-141">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="52647-142">contactId</span><span class="sxs-lookup"><span data-stu-id="52647-142">contactId</span></span>|<span data-ttu-id="52647-143">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="52647-143">string, maximum size 250</span></span>|<span data-ttu-id="52647-144">Идентификатор контакта Exchange для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-144">The exchange contact id for the given customer.</span></span> <span data-ttu-id="52647-145">Если идентификатор клиента не указан, мы будем использовать идентификатор контакта, чтобы найти его.</span><span class="sxs-lookup"><span data-stu-id="52647-145">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="52647-146">Постингдате</span><span class="sxs-lookup"><span data-stu-id="52647-146">postingDate</span></span>|<span data-ttu-id="52647-147">date</span><span class="sxs-lookup"><span data-stu-id="52647-147">date</span></span>|<span data-ttu-id="52647-148">Дата, когда выполняется разноска платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-148">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="52647-149">Документнумбер</span><span class="sxs-lookup"><span data-stu-id="52647-149">documentNumber</span></span>|<span data-ttu-id="52647-150">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="52647-150">string, maximum size 20</span></span>|<span data-ttu-id="52647-151">Указывает номер документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-151">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="52647-152">Екстерналдокументнумбер</span><span class="sxs-lookup"><span data-stu-id="52647-152">externalDocumentNumber</span></span>|<span data-ttu-id="52647-153">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="52647-153">string, maximum size 20</span></span>|<span data-ttu-id="52647-154">Указывает номер внешнего документа для платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-154">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="52647-155">отступ</span><span class="sxs-lookup"><span data-stu-id="52647-155">amount</span></span>|<span data-ttu-id="52647-156">числе</span><span class="sxs-lookup"><span data-stu-id="52647-156">decimal</span></span>|<span data-ttu-id="52647-157">Указывает общую сумму (включая НДС), из которой состоит платеж клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-157">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="52647-158">Апплиестоинвоицеид</span><span class="sxs-lookup"><span data-stu-id="52647-158">appliesToInvoiceId</span></span>|<span data-ttu-id="52647-159">GUID</span><span class="sxs-lookup"><span data-stu-id="52647-159">GUID</span></span>|<span data-ttu-id="52647-160">Уникальный идентификатор счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="52647-160">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="52647-161">Апплиестоинвоиценумбер</span><span class="sxs-lookup"><span data-stu-id="52647-161">appliesToInvoiceNumber</span></span>|<span data-ttu-id="52647-162">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="52647-162">string, maximum size 20</span></span>|<span data-ttu-id="52647-163">Номер счета, с которым связана оплата.</span><span class="sxs-lookup"><span data-stu-id="52647-163">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="52647-164">description</span><span class="sxs-lookup"><span data-stu-id="52647-164">description</span></span>|<span data-ttu-id="52647-165">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="52647-165">string, maximum size 50</span></span>|<span data-ttu-id="52647-166">Описание платежа клиента, предоставленное пользователем или созданным пользователем.</span><span class="sxs-lookup"><span data-stu-id="52647-166">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="52647-167">комментарий</span><span class="sxs-lookup"><span data-stu-id="52647-167">comment</span></span>|<span data-ttu-id="52647-168">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="52647-168">string, maximum size 250</span></span>|<span data-ttu-id="52647-169">Указанный пользователем комментарий к платежу клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-169">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="52647-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52647-170">lastModifiedDateTime</span></span>|<span data-ttu-id="52647-171">отличным</span><span class="sxs-lookup"><span data-stu-id="52647-171">datetime</span></span>|<span data-ttu-id="52647-172">Дата и время последнего изменения платежа клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-172">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="52647-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="52647-173">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="52647-174">Связи</span><span class="sxs-lookup"><span data-stu-id="52647-174">Relationships</span></span>
<span data-ttu-id="52647-175">Платеж клиента — это вложенная страница журнала платежей клиента.</span><span class="sxs-lookup"><span data-stu-id="52647-175">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="52647-176">Прямой доступ к нему невозможен.</span><span class="sxs-lookup"><span data-stu-id="52647-176">It cannot be accessed directly.</span></span>

<span data-ttu-id="52647-177">Платеж клиента может быть "родительским объектом" строк измерения.</span><span class="sxs-lookup"><span data-stu-id="52647-177">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="52647-178">Клиент (customerId) должен существовать в таблице Customers (клиенты).</span><span class="sxs-lookup"><span data-stu-id="52647-178">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="52647-179">Счет (Апплиестоинвоицеид) должен существовать в таблице "счета продаж".</span><span class="sxs-lookup"><span data-stu-id="52647-179">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="52647-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52647-180">JSON representation</span></span>

<span data-ttu-id="52647-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52647-181">Here is a JSON representation of the resource.</span></span>

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

