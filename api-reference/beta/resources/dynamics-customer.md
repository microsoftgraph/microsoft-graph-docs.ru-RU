---
title: Тип ресурса Customers
description: Представляет пользователя в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e4daa28018001fb6cb6e4866bedf8e256a72abef
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365936"
---
# <a name="customers-resource-type"></a><span data-ttu-id="46f09-103">Тип ресурса Customers</span><span class="sxs-lookup"><span data-stu-id="46f09-103">customers resource type</span></span>
<span data-ttu-id="46f09-104">Представляет пользователя в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="46f09-104">Represents a customer in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="46f09-105">Методы</span><span class="sxs-lookup"><span data-stu-id="46f09-105">Methods</span></span>

| <span data-ttu-id="46f09-106">Метод</span><span class="sxs-lookup"><span data-stu-id="46f09-106">Method</span></span>                                              |<span data-ttu-id="46f09-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="46f09-107">Return Type</span></span>| <span data-ttu-id="46f09-108">Описание</span><span class="sxs-lookup"><span data-stu-id="46f09-108">Description</span></span>      |
|:----------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="46f09-109">Получение клиентов</span><span class="sxs-lookup"><span data-stu-id="46f09-109">Get customers</span></span>](../api/dynamics-customer-get.md)      |<span data-ttu-id="46f09-110">TAP</span><span class="sxs-lookup"><span data-stu-id="46f09-110">customers</span></span>   |<span data-ttu-id="46f09-111">Получает клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-111">Gets a customer.</span></span>   |
|[<span data-ttu-id="46f09-112">Создание клиентов</span><span class="sxs-lookup"><span data-stu-id="46f09-112">Create customers</span></span>](../api/dynamics-create-customer.md)|<span data-ttu-id="46f09-113">TAP</span><span class="sxs-lookup"><span data-stu-id="46f09-113">customers</span></span>   |<span data-ttu-id="46f09-114">Создает клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-114">Creates a customer.</span></span>|
|[<span data-ttu-id="46f09-115">Обновление клиентов</span><span class="sxs-lookup"><span data-stu-id="46f09-115">Update customers</span></span>](../api/dynamics-customer-update.md)|<span data-ttu-id="46f09-116">TAP</span><span class="sxs-lookup"><span data-stu-id="46f09-116">customers</span></span>   |<span data-ttu-id="46f09-117">Обновляет клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-117">Updates a customer.</span></span>|
|[<span data-ttu-id="46f09-118">Удаление клиентов</span><span class="sxs-lookup"><span data-stu-id="46f09-118">Delete customers</span></span>](../api/dynamics-customer-delete.md)|<span data-ttu-id="46f09-119">Нет</span><span class="sxs-lookup"><span data-stu-id="46f09-119">none</span></span>        |<span data-ttu-id="46f09-120">Удаляет клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-120">Deletes a customer.</span></span>|

## <a name="properties"></a><span data-ttu-id="46f09-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="46f09-121">Properties</span></span>
| <span data-ttu-id="46f09-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="46f09-122">Property</span></span>    | <span data-ttu-id="46f09-123">Тип</span><span class="sxs-lookup"><span data-stu-id="46f09-123">Type</span></span>     |<span data-ttu-id="46f09-124">Описание</span><span class="sxs-lookup"><span data-stu-id="46f09-124">Description</span></span>|
|:------------|:---------|:----------|
|<span data-ttu-id="46f09-125">id</span><span class="sxs-lookup"><span data-stu-id="46f09-125">id</span></span>           |<span data-ttu-id="46f09-126">GUID</span><span class="sxs-lookup"><span data-stu-id="46f09-126">GUID</span></span>      |<span data-ttu-id="46f09-127">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="46f09-127">The unique ID of the item.</span></span> <span data-ttu-id="46f09-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="46f09-128">Non-editable.</span></span>|
|<span data-ttu-id="46f09-129">number</span><span class="sxs-lookup"><span data-stu-id="46f09-129">number</span></span>       |<span data-ttu-id="46f09-130">строка</span><span class="sxs-lookup"><span data-stu-id="46f09-130">string</span></span>    |<span data-ttu-id="46f09-131">Номер клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-131">The customer number.</span></span>|
|<span data-ttu-id="46f09-132">displayName</span><span class="sxs-lookup"><span data-stu-id="46f09-132">displayName</span></span>  |<span data-ttu-id="46f09-133">строка</span><span class="sxs-lookup"><span data-stu-id="46f09-133">string</span></span>    |<span data-ttu-id="46f09-134">Указывает имя клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-134">Specifies the customer's name.</span></span> <span data-ttu-id="46f09-135">Это имя будет отображаться во всех документах продажи для клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-135">This name will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="46f09-136">type</span><span class="sxs-lookup"><span data-stu-id="46f09-136">type</span></span>         |<span data-ttu-id="46f09-137">строка</span><span class="sxs-lookup"><span data-stu-id="46f09-137">string</span></span>    |<span data-ttu-id="46f09-138">Указывает тип клиента, который может иметь значение "Company" или "Person".</span><span class="sxs-lookup"><span data-stu-id="46f09-138">Specifies the type of customer, can be "Company" or "Person".</span></span>|
|<span data-ttu-id="46f09-139">address</span><span class="sxs-lookup"><span data-stu-id="46f09-139">address</span></span>      |[<span data-ttu-id="46f09-140">Навигационная. Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="46f09-140">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="46f09-141">Указывает адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-141">Specifies the customer's address.</span></span> <span data-ttu-id="46f09-142">Этот адрес будет отображаться во всех документах продажи для клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-142">This address will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="46f09-143">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="46f09-143">phoneNumber</span></span>  |<span data-ttu-id="46f09-144">строка</span><span class="sxs-lookup"><span data-stu-id="46f09-144">string</span></span>    |<span data-ttu-id="46f09-145">Указывает номер телефона клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-145">Specifies the customer's telephone number.</span></span>|
|<span data-ttu-id="46f09-146">email</span><span class="sxs-lookup"><span data-stu-id="46f09-146">email</span></span>        |<span data-ttu-id="46f09-147">строка</span><span class="sxs-lookup"><span data-stu-id="46f09-147">string</span></span>    |<span data-ttu-id="46f09-148">Указывает адрес электронной почты клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-148">Specifies the customer's email address.</span></span>|
|<span data-ttu-id="46f09-149">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="46f09-149">website</span></span>      |<span data-ttu-id="46f09-150">строка</span><span class="sxs-lookup"><span data-stu-id="46f09-150">string</span></span>    |<span data-ttu-id="46f09-151">Указывает адрес домашней страницы клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-151">Specifies the customer's home page address.</span></span>|
|<span data-ttu-id="46f09-152">Такслиабле</span><span class="sxs-lookup"><span data-stu-id="46f09-152">taxLiable</span></span>    |<span data-ttu-id="46f09-153">boolean</span><span class="sxs-lookup"><span data-stu-id="46f09-153">boolean</span></span>   |<span data-ttu-id="46f09-154">Указывает, несет ли клиент или поставщик налог на продажи.</span><span class="sxs-lookup"><span data-stu-id="46f09-154">Specifies if the customer or vendor is liable for sales tax.</span></span> <span data-ttu-id="46f09-155">Установите значение **true** , если клиент является налоговым.</span><span class="sxs-lookup"><span data-stu-id="46f09-155">Set to **true** if the customer is tax liable.</span></span>|
|<span data-ttu-id="46f09-156">Таксареаид</span><span class="sxs-lookup"><span data-stu-id="46f09-156">taxAreaId</span></span>    |<span data-ttu-id="46f09-157">GUID</span><span class="sxs-lookup"><span data-stu-id="46f09-157">GUID</span></span>      |<span data-ttu-id="46f09-158">Указывает, к какой налоговой области относится клиент.</span><span class="sxs-lookup"><span data-stu-id="46f09-158">Specifies which tax area the customer belongs to.</span></span>|
|<span data-ttu-id="46f09-159">Таксареадисплайнаме</span><span class="sxs-lookup"><span data-stu-id="46f09-159">taxAreaDisplayName</span></span>|<span data-ttu-id="46f09-160">строка</span><span class="sxs-lookup"><span data-stu-id="46f09-160">string</span></span>|<span data-ttu-id="46f09-161">Задает отображаемое имя налоговой области, к которой принадлежит клиент.</span><span class="sxs-lookup"><span data-stu-id="46f09-161">Specified the display name of the tax area the customer belongs to.</span></span>|
|<span data-ttu-id="46f09-162">Таксрегистратионнумбер</span><span class="sxs-lookup"><span data-stu-id="46f09-162">taxRegistrationNumber</span></span>|<span data-ttu-id="46f09-163">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="46f09-163">string, maximum size 20</span></span>|<span data-ttu-id="46f09-164">Указывается регистрационный номер налогоплательщика для клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-164">Specified the tax registration number of the customer.</span></span>|
|<span data-ttu-id="46f09-165">Курренциид</span><span class="sxs-lookup"><span data-stu-id="46f09-165">currencyId</span></span>   |<span data-ttu-id="46f09-166">GUID</span><span class="sxs-lookup"><span data-stu-id="46f09-166">GUID</span></span>      |<span data-ttu-id="46f09-167">Указывает, какая валюта используется клиентом.</span><span class="sxs-lookup"><span data-stu-id="46f09-167">Specifies which currency the customer uses.</span></span>|
|<span data-ttu-id="46f09-168">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="46f09-168">currencyCode</span></span> |<span data-ttu-id="46f09-169">числовых</span><span class="sxs-lookup"><span data-stu-id="46f09-169">numeric</span></span>   |<span data-ttu-id="46f09-170">Код валюты по умолчанию для клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-170">The default currency code for the customer.</span></span>|
|<span data-ttu-id="46f09-171">Пайменттермсид</span><span class="sxs-lookup"><span data-stu-id="46f09-171">paymentTermsId</span></span>|<span data-ttu-id="46f09-172">GUID</span><span class="sxs-lookup"><span data-stu-id="46f09-172">GUID</span></span>     |<span data-ttu-id="46f09-173">Указывает, какой термин оплаты использует клиент.</span><span class="sxs-lookup"><span data-stu-id="46f09-173">Specifies which payment term the customer uses.</span></span>|
|<span data-ttu-id="46f09-174">Пайментмесодид</span><span class="sxs-lookup"><span data-stu-id="46f09-174">paymentMethodId</span></span>|<span data-ttu-id="46f09-175">GUID</span><span class="sxs-lookup"><span data-stu-id="46f09-175">GUID</span></span>    |<span data-ttu-id="46f09-176">Указывает, какой метод оплаты используется клиентом.</span><span class="sxs-lookup"><span data-stu-id="46f09-176">Specifies which payment method the customer uses.</span></span>|
|<span data-ttu-id="46f09-177">Шипментмесодид</span><span class="sxs-lookup"><span data-stu-id="46f09-177">shipmentMethodId</span></span>|<span data-ttu-id="46f09-178">GUID</span><span class="sxs-lookup"><span data-stu-id="46f09-178">GUID</span></span>   |<span data-ttu-id="46f09-179">Указывает метод отгрузки, используемый клиентом.</span><span class="sxs-lookup"><span data-stu-id="46f09-179">Specifies which shipment method the customer uses.</span></span>|
|<span data-ttu-id="46f09-180">заблокировано</span><span class="sxs-lookup"><span data-stu-id="46f09-180">blocked</span></span>      |<span data-ttu-id="46f09-181">строка</span><span class="sxs-lookup"><span data-stu-id="46f09-181">string</span></span>    |<span data-ttu-id="46f09-182">Указывает, что транзакции с клиентом не могут быть учтены.</span><span class="sxs-lookup"><span data-stu-id="46f09-182">Specifies that transactions with the customer cannot be posted.</span></span> <span data-ttu-id="46f09-183">Значение " **все**", если клиент заблокирован, имеет значение "пусто", если оно не заблокировано.</span><span class="sxs-lookup"><span data-stu-id="46f09-183">Set to **All**, if the customer is blocked, set to blank if not blocked.</span></span>|
|<span data-ttu-id="46f09-184">равномерно</span><span class="sxs-lookup"><span data-stu-id="46f09-184">balance</span></span>      |<span data-ttu-id="46f09-185">числовых</span><span class="sxs-lookup"><span data-stu-id="46f09-185">numeric</span></span>   |<span data-ttu-id="46f09-186">Сумма платежа, которую долг клиенту соответствует выполненным продажам.</span><span class="sxs-lookup"><span data-stu-id="46f09-186">Specifies the payment amount that the customer owes for completed sales.</span></span> <span data-ttu-id="46f09-187">Это значение также называется балансом клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-187">This value is also known as the customer's balance.</span></span> <span data-ttu-id="46f09-188">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46f09-188">Read-Only.</span></span>|
|<span data-ttu-id="46f09-189">Овердуеамаунт</span><span class="sxs-lookup"><span data-stu-id="46f09-189">overdueAmount</span></span>|<span data-ttu-id="46f09-190">числовых</span><span class="sxs-lookup"><span data-stu-id="46f09-190">numeric</span></span>   |<span data-ttu-id="46f09-191">Указывает просроченное значение клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-191">Specifies the customer's overdue amount.</span></span>|
|<span data-ttu-id="46f09-192">Тоталсалесексклудингтакс</span><span class="sxs-lookup"><span data-stu-id="46f09-192">totalSalesExcludingTax</span></span>|<span data-ttu-id="46f09-193">числовых</span><span class="sxs-lookup"><span data-stu-id="46f09-193">numeric</span></span>|<span data-ttu-id="46f09-194">Указывает общую сумму продаж, исключая налог для клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-194">Specifies the total sales amount excluding tax of the customer.</span></span>|
|<span data-ttu-id="46f09-195">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46f09-195">lastModifiedDateTime</span></span>|<span data-ttu-id="46f09-196">отличным</span><span class="sxs-lookup"><span data-stu-id="46f09-196">datetime</span></span>|<span data-ttu-id="46f09-197">Дата и время последнего изменения клиента.</span><span class="sxs-lookup"><span data-stu-id="46f09-197">The last datetime the customer was modified.</span></span> <span data-ttu-id="46f09-198">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46f09-198">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="46f09-199">Отношения</span><span class="sxs-lookup"><span data-stu-id="46f09-199">Relationships</span></span>
<span data-ttu-id="46f09-200">Валюта (Курренцикоде) должна существовать в таблице валюты.</span><span class="sxs-lookup"><span data-stu-id="46f09-200">A Currency(currencyCode) must exist in the Currencies table.</span></span>

<span data-ttu-id="46f09-201">Срок платежа (Пайменттермс) должен существовать в таблице формула оплаты.</span><span class="sxs-lookup"><span data-stu-id="46f09-201">A Payment Term(paymentTerms) must exist in the Payment Terms table.</span></span>

<span data-ttu-id="46f09-202">Метод отГрузки (Шипментмесод) должен существовать в таблице метод отГрузки.</span><span class="sxs-lookup"><span data-stu-id="46f09-202">A Shipment Method(shipmentMethod) must exist in the Shipment Method table.</span></span>

<span data-ttu-id="46f09-203">Метод оплаты (Пайментмесод) должен существовать в таблице метод оплаты.</span><span class="sxs-lookup"><span data-stu-id="46f09-203">A Payment Method(paymentMethod) must exist in the Payment Method table.</span></span>

<span data-ttu-id="46f09-204">Налоговая область (Таксареа) должна существовать в таблице налоговая область.</span><span class="sxs-lookup"><span data-stu-id="46f09-204">A Tax Area(taxArea) must exist in the Tax Area table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46f09-205">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="46f09-205">JSON representation</span></span>

<span data-ttu-id="46f09-206">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46f09-206">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "address": NAV.PostalAddress,
    "phoneNumber": "string",
    "email": "string",
    "website": "string",
    "taxLiable": "boolean",
    "taxAreaId": "GUID",
    "taxAreaDisplayName": "string",
    "taxRegistrationNumber": "string",
    "currencyCode": "string",
    "paymentTermsId": "GUID",
    "shipmentMethodId": "GUID",
    "paymentMethodId":  "GUID",
    "blocked": "string",
    "balance": "decimal",
    "overdueAmount": "numeric",
    "totalSalesExcludingTax": "numeric",
    "lastModifiedDateTime": "datetime"
}


```

