---
title: Тип ресурса "поставщики"
description: Объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1cec20dee4a124bb704d60ceb8229ea820aa55b0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365663"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="5c457-103">Тип ресурса "поставщики"</span><span class="sxs-lookup"><span data-stu-id="5c457-103">vendors resource type</span></span>
<span data-ttu-id="5c457-104">Представляет поставщика в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="5c457-104">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="5c457-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5c457-105">Methods</span></span>

| <span data-ttu-id="5c457-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5c457-106">Method</span></span>       | <span data-ttu-id="5c457-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c457-107">Return Type</span></span>  |<span data-ttu-id="5c457-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5c457-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c457-109">Получение поставщиков</span><span class="sxs-lookup"><span data-stu-id="5c457-109">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="5c457-110">поставщиков</span><span class="sxs-lookup"><span data-stu-id="5c457-110">vendors</span></span>|<span data-ttu-id="5c457-111">Возвращает объект Vendor.</span><span class="sxs-lookup"><span data-stu-id="5c457-111">Gets a vendor object.</span></span>|
|[<span data-ttu-id="5c457-112">Учет поставщиков</span><span class="sxs-lookup"><span data-stu-id="5c457-112">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="5c457-113">поставщиков</span><span class="sxs-lookup"><span data-stu-id="5c457-113">vendors</span></span>|<span data-ttu-id="5c457-114">Создает объект Vendor.</span><span class="sxs-lookup"><span data-stu-id="5c457-114">Creates a vendor object.</span></span>|
|[<span data-ttu-id="5c457-115">Поставщики обновлений</span><span class="sxs-lookup"><span data-stu-id="5c457-115">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="5c457-116">поставщиков</span><span class="sxs-lookup"><span data-stu-id="5c457-116">vendors</span></span>|<span data-ttu-id="5c457-117">Обновляет объект Vendor.</span><span class="sxs-lookup"><span data-stu-id="5c457-117">Updates a vendor object.</span></span>|
|[<span data-ttu-id="5c457-118">Удаление поставщика</span><span class="sxs-lookup"><span data-stu-id="5c457-118">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="5c457-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5c457-119">none</span></span>|<span data-ttu-id="5c457-120">Удаляет объект Vendor.</span><span class="sxs-lookup"><span data-stu-id="5c457-120">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c457-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c457-121">Properties</span></span>
| <span data-ttu-id="5c457-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c457-122">Property</span></span>     | <span data-ttu-id="5c457-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5c457-123">Type</span></span>   |<span data-ttu-id="5c457-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5c457-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c457-125">id</span><span class="sxs-lookup"><span data-stu-id="5c457-125">id</span></span>|<span data-ttu-id="5c457-126">GUID</span><span class="sxs-lookup"><span data-stu-id="5c457-126">GUID</span></span>|<span data-ttu-id="5c457-127">Уникальный идентификатор поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-127">The unique ID of the vendor.</span></span> <span data-ttu-id="5c457-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="5c457-128">Non-editable.</span></span>|
|<span data-ttu-id="5c457-129">number</span><span class="sxs-lookup"><span data-stu-id="5c457-129">number</span></span>|<span data-ttu-id="5c457-130">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-130">string</span></span>|<span data-ttu-id="5c457-131">Номер поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-131">The vendor number.</span></span>|
|<span data-ttu-id="5c457-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5c457-132">displayName</span></span>|<span data-ttu-id="5c457-133">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-133">string</span></span>|<span data-ttu-id="5c457-134">Отображаемое имя поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-134">The vendor's display name.</span></span>|
|<span data-ttu-id="5c457-135">address</span><span class="sxs-lookup"><span data-stu-id="5c457-135">address</span></span>|[<span data-ttu-id="5c457-136">Навигационная. Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="5c457-136">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="5c457-137">Адрес поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-137">The vendor's address.</span></span>|
|<span data-ttu-id="5c457-138">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="5c457-138">phoneNumber</span></span>|<span data-ttu-id="5c457-139">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-139">string</span></span>|<span data-ttu-id="5c457-140">Номер телефона поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-140">The vendor's telephone number.</span></span>|
|<span data-ttu-id="5c457-141">email</span><span class="sxs-lookup"><span data-stu-id="5c457-141">email</span></span>|<span data-ttu-id="5c457-142">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-142">string</span></span>|<span data-ttu-id="5c457-143">Адрес электронной почты поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-143">The vendor's email address.</span></span>|
|<span data-ttu-id="5c457-144">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="5c457-144">website</span></span>|<span data-ttu-id="5c457-145">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-145">string</span></span>|<span data-ttu-id="5c457-146">Адрес веб-сайта поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-146">The vendor's website address.</span></span>|
|<span data-ttu-id="5c457-147">Таксрегистратионнумбер</span><span class="sxs-lookup"><span data-stu-id="5c457-147">taxRegistrationNumber</span></span>|<span data-ttu-id="5c457-148">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-148">string</span></span>|<span data-ttu-id="5c457-149">Регистрационный номер налогоплательщика поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-149">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="5c457-150">Курренциид</span><span class="sxs-lookup"><span data-stu-id="5c457-150">currencyId</span></span>|<span data-ttu-id="5c457-151">GUID</span><span class="sxs-lookup"><span data-stu-id="5c457-151">GUID</span></span>|<span data-ttu-id="5c457-152">Идентификатор кода валюты по умолчанию для поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-152">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="5c457-153">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="5c457-153">currencyCode</span></span>|<span data-ttu-id="5c457-154">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-154">string</span></span>|<span data-ttu-id="5c457-155">Код валюты по умолчанию для поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-155">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="5c457-156">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="5c457-156">irs1099Code</span></span>|<span data-ttu-id="5c457-157">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-157">string</span></span>|<span data-ttu-id="5c457-158">Указывает код 1099 для поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-158">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="5c457-159">Только для США.</span><span class="sxs-lookup"><span data-stu-id="5c457-159">US only.</span></span>|
|<span data-ttu-id="5c457-160">Пайменттермсид</span><span class="sxs-lookup"><span data-stu-id="5c457-160">paymentTermsId</span></span>|<span data-ttu-id="5c457-161">GUID</span><span class="sxs-lookup"><span data-stu-id="5c457-161">GUID</span></span>|<span data-ttu-id="5c457-162">КОД условий оплаты для поставщика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5c457-162">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="5c457-163">Пайментмесодид</span><span class="sxs-lookup"><span data-stu-id="5c457-163">paymentMethodId</span></span>|<span data-ttu-id="5c457-164">GUID</span><span class="sxs-lookup"><span data-stu-id="5c457-164">GUID</span></span>|<span data-ttu-id="5c457-165">Идентификатор метода оплаты по умолчанию для поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-165">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="5c457-166">Такслиабле</span><span class="sxs-lookup"><span data-stu-id="5c457-166">taxLiable</span></span>|<span data-ttu-id="5c457-167">boolean</span><span class="sxs-lookup"><span data-stu-id="5c457-167">boolean</span></span>|<span data-ttu-id="5c457-168">Указывает, является ли поставщик подлежащей налогообложению.</span><span class="sxs-lookup"><span data-stu-id="5c457-168">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="5c457-169">заблокировано</span><span class="sxs-lookup"><span data-stu-id="5c457-169">blocked</span></span>|<span data-ttu-id="5c457-170">строка</span><span class="sxs-lookup"><span data-stu-id="5c457-170">string</span></span>|<span data-ttu-id="5c457-171">Указывает, какие транзакции у поставщика, который не может быть разнесен.</span><span class="sxs-lookup"><span data-stu-id="5c457-171">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="5c457-172">Допустимые значения: пусто, оплата или все</span><span class="sxs-lookup"><span data-stu-id="5c457-172">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="5c457-173">равномерно</span><span class="sxs-lookup"><span data-stu-id="5c457-173">balance</span></span>|<span data-ttu-id="5c457-174">числе</span><span class="sxs-lookup"><span data-stu-id="5c457-174">decimal</span></span>|<span data-ttu-id="5c457-175">Сальдо поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-175">The vendor's balance.</span></span> <span data-ttu-id="5c457-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c457-176">Read-Only.</span></span>|
|<span data-ttu-id="5c457-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c457-177">lastModifiedDateTime</span></span>|<span data-ttu-id="5c457-178">отличным</span><span class="sxs-lookup"><span data-stu-id="5c457-178">datetime</span></span>|<span data-ttu-id="5c457-179">Дата и время последнего изменения поставщика.</span><span class="sxs-lookup"><span data-stu-id="5c457-179">The last datetime the vendor was modified.</span></span> <span data-ttu-id="5c457-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c457-180">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="5c457-181">Отношения</span><span class="sxs-lookup"><span data-stu-id="5c457-181">Relationships</span></span>
<span data-ttu-id="5c457-182">Нет</span><span class="sxs-lookup"><span data-stu-id="5c457-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c457-183">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5c457-183">JSON representation</span></span>

<span data-ttu-id="5c457-184">Ниже показано представление поставщика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c457-184">Here is a JSON representation of the vendor.</span></span>

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

