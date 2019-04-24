---
title: Тип ресурса Customers
description: Представляет пользователя в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e4daa28018001fb6cb6e4866bedf8e256a72abef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507261"
---
# <a name="customers-resource-type"></a><span data-ttu-id="f7964-103">Тип ресурса Customers</span><span class="sxs-lookup"><span data-stu-id="f7964-103">customers resource type</span></span>
<span data-ttu-id="f7964-104">Представляет пользователя в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f7964-104">Represents a customer in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f7964-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f7964-105">Methods</span></span>

| <span data-ttu-id="f7964-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f7964-106">Method</span></span>                                              |<span data-ttu-id="f7964-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7964-107">Return Type</span></span>| <span data-ttu-id="f7964-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f7964-108">Description</span></span>      |
|:----------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="f7964-109">Получение клиентов</span><span class="sxs-lookup"><span data-stu-id="f7964-109">Get customers</span></span>](../api/dynamics-customer-get.md)      |<span data-ttu-id="f7964-110">TAP</span><span class="sxs-lookup"><span data-stu-id="f7964-110">customers</span></span>   |<span data-ttu-id="f7964-111">Получает клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-111">Gets a customer.</span></span>   |
|[<span data-ttu-id="f7964-112">Создание клиентов</span><span class="sxs-lookup"><span data-stu-id="f7964-112">Create customers</span></span>](../api/dynamics-create-customer.md)|<span data-ttu-id="f7964-113">TAP</span><span class="sxs-lookup"><span data-stu-id="f7964-113">customers</span></span>   |<span data-ttu-id="f7964-114">Создает клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-114">Creates a customer.</span></span>|
|[<span data-ttu-id="f7964-115">Обновление клиентов</span><span class="sxs-lookup"><span data-stu-id="f7964-115">Update customers</span></span>](../api/dynamics-customer-update.md)|<span data-ttu-id="f7964-116">TAP</span><span class="sxs-lookup"><span data-stu-id="f7964-116">customers</span></span>   |<span data-ttu-id="f7964-117">Обновляет клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-117">Updates a customer.</span></span>|
|[<span data-ttu-id="f7964-118">Удаление клиентов</span><span class="sxs-lookup"><span data-stu-id="f7964-118">Delete customers</span></span>](../api/dynamics-customer-delete.md)|<span data-ttu-id="f7964-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f7964-119">none</span></span>        |<span data-ttu-id="f7964-120">Удаляет клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-120">Deletes a customer.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7964-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7964-121">Properties</span></span>
| <span data-ttu-id="f7964-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7964-122">Property</span></span>    | <span data-ttu-id="f7964-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f7964-123">Type</span></span>     |<span data-ttu-id="f7964-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f7964-124">Description</span></span>|
|:------------|:---------|:----------|
|<span data-ttu-id="f7964-125">id</span><span class="sxs-lookup"><span data-stu-id="f7964-125">id</span></span>           |<span data-ttu-id="f7964-126">GUID</span><span class="sxs-lookup"><span data-stu-id="f7964-126">GUID</span></span>      |<span data-ttu-id="f7964-127">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="f7964-127">The unique ID of the item.</span></span> <span data-ttu-id="f7964-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="f7964-128">Non-editable.</span></span>|
|<span data-ttu-id="f7964-129">number</span><span class="sxs-lookup"><span data-stu-id="f7964-129">number</span></span>       |<span data-ttu-id="f7964-130">строка</span><span class="sxs-lookup"><span data-stu-id="f7964-130">string</span></span>    |<span data-ttu-id="f7964-131">Номер клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-131">The customer number.</span></span>|
|<span data-ttu-id="f7964-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f7964-132">displayName</span></span>  |<span data-ttu-id="f7964-133">string</span><span class="sxs-lookup"><span data-stu-id="f7964-133">string</span></span>    |<span data-ttu-id="f7964-134">Указывает имя клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-134">Specifies the customer's name.</span></span> <span data-ttu-id="f7964-135">Это имя будет отображаться во всех документах продажи для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-135">This name will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="f7964-136">type</span><span class="sxs-lookup"><span data-stu-id="f7964-136">type</span></span>         |<span data-ttu-id="f7964-137">string</span><span class="sxs-lookup"><span data-stu-id="f7964-137">string</span></span>    |<span data-ttu-id="f7964-138">Указывает тип клиента, который может иметь значение "Company" или "Person".</span><span class="sxs-lookup"><span data-stu-id="f7964-138">Specifies the type of customer, can be "Company" or "Person".</span></span>|
|<span data-ttu-id="f7964-139">address</span><span class="sxs-lookup"><span data-stu-id="f7964-139">address</span></span>      |[<span data-ttu-id="f7964-140">Навигационная. Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="f7964-140">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="f7964-141">Указывает адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-141">Specifies the customer's address.</span></span> <span data-ttu-id="f7964-142">Этот адрес будет отображаться во всех документах продажи для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-142">This address will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="f7964-143">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f7964-143">phoneNumber</span></span>  |<span data-ttu-id="f7964-144">строка</span><span class="sxs-lookup"><span data-stu-id="f7964-144">string</span></span>    |<span data-ttu-id="f7964-145">Указывает номер телефона клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-145">Specifies the customer's telephone number.</span></span>|
|<span data-ttu-id="f7964-146">email</span><span class="sxs-lookup"><span data-stu-id="f7964-146">email</span></span>        |<span data-ttu-id="f7964-147">строка</span><span class="sxs-lookup"><span data-stu-id="f7964-147">string</span></span>    |<span data-ttu-id="f7964-148">Указывает адрес электронной почты клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-148">Specifies the customer's email address.</span></span>|
|<span data-ttu-id="f7964-149">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="f7964-149">website</span></span>      |<span data-ttu-id="f7964-150">строка</span><span class="sxs-lookup"><span data-stu-id="f7964-150">string</span></span>    |<span data-ttu-id="f7964-151">Указывает адрес домашней страницы клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-151">Specifies the customer's home page address.</span></span>|
|<span data-ttu-id="f7964-152">Такслиабле</span><span class="sxs-lookup"><span data-stu-id="f7964-152">taxLiable</span></span>    |<span data-ttu-id="f7964-153">логический</span><span class="sxs-lookup"><span data-stu-id="f7964-153">boolean</span></span>   |<span data-ttu-id="f7964-154">Указывает, несет ли клиент или поставщик налог на продажи.</span><span class="sxs-lookup"><span data-stu-id="f7964-154">Specifies if the customer or vendor is liable for sales tax.</span></span> <span data-ttu-id="f7964-155">Установите значение **true** , если клиент является налоговым.</span><span class="sxs-lookup"><span data-stu-id="f7964-155">Set to **true** if the customer is tax liable.</span></span>|
|<span data-ttu-id="f7964-156">Таксареаид</span><span class="sxs-lookup"><span data-stu-id="f7964-156">taxAreaId</span></span>    |<span data-ttu-id="f7964-157">GUID</span><span class="sxs-lookup"><span data-stu-id="f7964-157">GUID</span></span>      |<span data-ttu-id="f7964-158">Указывает, к какой налоговой области относится клиент.</span><span class="sxs-lookup"><span data-stu-id="f7964-158">Specifies which tax area the customer belongs to.</span></span>|
|<span data-ttu-id="f7964-159">Таксареадисплайнаме</span><span class="sxs-lookup"><span data-stu-id="f7964-159">taxAreaDisplayName</span></span>|<span data-ttu-id="f7964-160">строка</span><span class="sxs-lookup"><span data-stu-id="f7964-160">string</span></span>|<span data-ttu-id="f7964-161">Задает отображаемое имя налоговой области, к которой принадлежит клиент.</span><span class="sxs-lookup"><span data-stu-id="f7964-161">Specified the display name of the tax area the customer belongs to.</span></span>|
|<span data-ttu-id="f7964-162">Таксрегистратионнумбер</span><span class="sxs-lookup"><span data-stu-id="f7964-162">taxRegistrationNumber</span></span>|<span data-ttu-id="f7964-163">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="f7964-163">string, maximum size 20</span></span>|<span data-ttu-id="f7964-164">Указывается регистрационный номер налогоплательщика для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-164">Specified the tax registration number of the customer.</span></span>|
|<span data-ttu-id="f7964-165">Курренциид</span><span class="sxs-lookup"><span data-stu-id="f7964-165">currencyId</span></span>   |<span data-ttu-id="f7964-166">GUID</span><span class="sxs-lookup"><span data-stu-id="f7964-166">GUID</span></span>      |<span data-ttu-id="f7964-167">Указывает, какая валюта используется клиентом.</span><span class="sxs-lookup"><span data-stu-id="f7964-167">Specifies which currency the customer uses.</span></span>|
|<span data-ttu-id="f7964-168">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="f7964-168">currencyCode</span></span> |<span data-ttu-id="f7964-169">числовых</span><span class="sxs-lookup"><span data-stu-id="f7964-169">numeric</span></span>   |<span data-ttu-id="f7964-170">Код валюты по умолчанию для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-170">The default currency code for the customer.</span></span>|
|<span data-ttu-id="f7964-171">Пайменттермсид</span><span class="sxs-lookup"><span data-stu-id="f7964-171">paymentTermsId</span></span>|<span data-ttu-id="f7964-172">GUID</span><span class="sxs-lookup"><span data-stu-id="f7964-172">GUID</span></span>     |<span data-ttu-id="f7964-173">Указывает, какой термин оплаты использует клиент.</span><span class="sxs-lookup"><span data-stu-id="f7964-173">Specifies which payment term the customer uses.</span></span>|
|<span data-ttu-id="f7964-174">Пайментмесодид</span><span class="sxs-lookup"><span data-stu-id="f7964-174">paymentMethodId</span></span>|<span data-ttu-id="f7964-175">GUID</span><span class="sxs-lookup"><span data-stu-id="f7964-175">GUID</span></span>    |<span data-ttu-id="f7964-176">Указывает, какой метод оплаты используется клиентом.</span><span class="sxs-lookup"><span data-stu-id="f7964-176">Specifies which payment method the customer uses.</span></span>|
|<span data-ttu-id="f7964-177">Шипментмесодид</span><span class="sxs-lookup"><span data-stu-id="f7964-177">shipmentMethodId</span></span>|<span data-ttu-id="f7964-178">GUID</span><span class="sxs-lookup"><span data-stu-id="f7964-178">GUID</span></span>   |<span data-ttu-id="f7964-179">Указывает метод отгрузки, используемый клиентом.</span><span class="sxs-lookup"><span data-stu-id="f7964-179">Specifies which shipment method the customer uses.</span></span>|
|<span data-ttu-id="f7964-180">заблокированных</span><span class="sxs-lookup"><span data-stu-id="f7964-180">blocked</span></span>      |<span data-ttu-id="f7964-181">строка</span><span class="sxs-lookup"><span data-stu-id="f7964-181">string</span></span>    |<span data-ttu-id="f7964-182">Указывает, что транзакции с клиентом не могут быть учтены.</span><span class="sxs-lookup"><span data-stu-id="f7964-182">Specifies that transactions with the customer cannot be posted.</span></span> <span data-ttu-id="f7964-183">Значение " **все**", если клиент заблокирован, имеет значение "пусто", если оно не заблокировано.</span><span class="sxs-lookup"><span data-stu-id="f7964-183">Set to **All**, if the customer is blocked, set to blank if not blocked.</span></span>|
|<span data-ttu-id="f7964-184">равномерно</span><span class="sxs-lookup"><span data-stu-id="f7964-184">balance</span></span>      |<span data-ttu-id="f7964-185">числовых</span><span class="sxs-lookup"><span data-stu-id="f7964-185">numeric</span></span>   |<span data-ttu-id="f7964-186">Сумма платежа, которую долг клиенту соответствует выполненным продажам.</span><span class="sxs-lookup"><span data-stu-id="f7964-186">Specifies the payment amount that the customer owes for completed sales.</span></span> <span data-ttu-id="f7964-187">Это значение также называется балансом клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-187">This value is also known as the customer's balance.</span></span> <span data-ttu-id="f7964-188">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f7964-188">Read-Only.</span></span>|
|<span data-ttu-id="f7964-189">Овердуеамаунт</span><span class="sxs-lookup"><span data-stu-id="f7964-189">overdueAmount</span></span>|<span data-ttu-id="f7964-190">числовых</span><span class="sxs-lookup"><span data-stu-id="f7964-190">numeric</span></span>   |<span data-ttu-id="f7964-191">Указывает просроченное значение клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-191">Specifies the customer's overdue amount.</span></span>|
|<span data-ttu-id="f7964-192">Тоталсалесексклудингтакс</span><span class="sxs-lookup"><span data-stu-id="f7964-192">totalSalesExcludingTax</span></span>|<span data-ttu-id="f7964-193">числовых</span><span class="sxs-lookup"><span data-stu-id="f7964-193">numeric</span></span>|<span data-ttu-id="f7964-194">Указывает общую сумму продаж, исключая налог для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-194">Specifies the total sales amount excluding tax of the customer.</span></span>|
|<span data-ttu-id="f7964-195">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7964-195">lastModifiedDateTime</span></span>|<span data-ttu-id="f7964-196">отличным</span><span class="sxs-lookup"><span data-stu-id="f7964-196">datetime</span></span>|<span data-ttu-id="f7964-197">Дата и время последнего изменения клиента.</span><span class="sxs-lookup"><span data-stu-id="f7964-197">The last datetime the customer was modified.</span></span> <span data-ttu-id="f7964-198">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f7964-198">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="f7964-199">Связи</span><span class="sxs-lookup"><span data-stu-id="f7964-199">Relationships</span></span>
<span data-ttu-id="f7964-200">Валюта (Курренцикоде) должна существовать в таблице валюты.</span><span class="sxs-lookup"><span data-stu-id="f7964-200">A Currency(currencyCode) must exist in the Currencies table.</span></span>

<span data-ttu-id="f7964-201">Срок платежа (Пайменттермс) должен существовать в таблице формула оплаты.</span><span class="sxs-lookup"><span data-stu-id="f7964-201">A Payment Term(paymentTerms) must exist in the Payment Terms table.</span></span>

<span data-ttu-id="f7964-202">Метод отГрузки (Шипментмесод) должен существовать в таблице метод отГрузки.</span><span class="sxs-lookup"><span data-stu-id="f7964-202">A Shipment Method(shipmentMethod) must exist in the Shipment Method table.</span></span>

<span data-ttu-id="f7964-203">Метод оплаты (Пайментмесод) должен существовать в таблице метод оплаты.</span><span class="sxs-lookup"><span data-stu-id="f7964-203">A Payment Method(paymentMethod) must exist in the Payment Method table.</span></span>

<span data-ttu-id="f7964-204">Налоговая область (Таксареа) должна существовать в таблице налоговая область.</span><span class="sxs-lookup"><span data-stu-id="f7964-204">A Tax Area(taxArea) must exist in the Tax Area table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7964-205">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7964-205">JSON representation</span></span>

<span data-ttu-id="f7964-206">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7964-206">Here is a JSON representation of the resource.</span></span>


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

