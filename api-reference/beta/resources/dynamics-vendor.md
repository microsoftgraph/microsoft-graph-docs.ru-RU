---
title: Тип ресурса "поставщики"
description: Объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7c0609d96f6d97503faf5c5251d3641979a4f6e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972854"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="df79c-103">Тип ресурса "поставщики"</span><span class="sxs-lookup"><span data-stu-id="df79c-103">vendors resource type</span></span>
<span data-ttu-id="df79c-104">Представляет поставщика в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="df79c-104">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="df79c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="df79c-105">Methods</span></span>

| <span data-ttu-id="df79c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="df79c-106">Method</span></span>       | <span data-ttu-id="df79c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="df79c-107">Return Type</span></span>  |<span data-ttu-id="df79c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="df79c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df79c-109">Получение поставщиков</span><span class="sxs-lookup"><span data-stu-id="df79c-109">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="df79c-110">поставщиков</span><span class="sxs-lookup"><span data-stu-id="df79c-110">vendors</span></span>|<span data-ttu-id="df79c-111">Возвращает объект Vendor.</span><span class="sxs-lookup"><span data-stu-id="df79c-111">Gets a vendor object.</span></span>|
|[<span data-ttu-id="df79c-112">Учет поставщиков</span><span class="sxs-lookup"><span data-stu-id="df79c-112">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="df79c-113">поставщиков</span><span class="sxs-lookup"><span data-stu-id="df79c-113">vendors</span></span>|<span data-ttu-id="df79c-114">Создает объект Vendor.</span><span class="sxs-lookup"><span data-stu-id="df79c-114">Creates a vendor object.</span></span>|
|[<span data-ttu-id="df79c-115">Поставщики обновлений</span><span class="sxs-lookup"><span data-stu-id="df79c-115">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="df79c-116">поставщиков</span><span class="sxs-lookup"><span data-stu-id="df79c-116">vendors</span></span>|<span data-ttu-id="df79c-117">Обновляет объект Vendor.</span><span class="sxs-lookup"><span data-stu-id="df79c-117">Updates a vendor object.</span></span>|
|[<span data-ttu-id="df79c-118">Удаление поставщика</span><span class="sxs-lookup"><span data-stu-id="df79c-118">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="df79c-119">none</span><span class="sxs-lookup"><span data-stu-id="df79c-119">none</span></span>|<span data-ttu-id="df79c-120">Удаляет объект Vendor.</span><span class="sxs-lookup"><span data-stu-id="df79c-120">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="df79c-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="df79c-121">Properties</span></span>
| <span data-ttu-id="df79c-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="df79c-122">Property</span></span>     | <span data-ttu-id="df79c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="df79c-123">Type</span></span>   |<span data-ttu-id="df79c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="df79c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df79c-125">id</span><span class="sxs-lookup"><span data-stu-id="df79c-125">id</span></span>|<span data-ttu-id="df79c-126">GUID</span><span class="sxs-lookup"><span data-stu-id="df79c-126">GUID</span></span>|<span data-ttu-id="df79c-127">Уникальный идентификатор поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-127">The unique ID of the vendor.</span></span> <span data-ttu-id="df79c-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="df79c-128">Non-editable.</span></span>|
|<span data-ttu-id="df79c-129">число</span><span class="sxs-lookup"><span data-stu-id="df79c-129">number</span></span>|<span data-ttu-id="df79c-130">string</span><span class="sxs-lookup"><span data-stu-id="df79c-130">string</span></span>|<span data-ttu-id="df79c-131">Номер поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-131">The vendor number.</span></span>|
|<span data-ttu-id="df79c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="df79c-132">displayName</span></span>|<span data-ttu-id="df79c-133">string</span><span class="sxs-lookup"><span data-stu-id="df79c-133">string</span></span>|<span data-ttu-id="df79c-134">Отображаемое имя поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-134">The vendor's display name.</span></span>|
|<span data-ttu-id="df79c-135">address</span><span class="sxs-lookup"><span data-stu-id="df79c-135">address</span></span>|[<span data-ttu-id="df79c-136">Навигационная. Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="df79c-136">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="df79c-137">Адрес поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-137">The vendor's address.</span></span>|
|<span data-ttu-id="df79c-138">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="df79c-138">phoneNumber</span></span>|<span data-ttu-id="df79c-139">string</span><span class="sxs-lookup"><span data-stu-id="df79c-139">string</span></span>|<span data-ttu-id="df79c-140">Номер телефона поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-140">The vendor's telephone number.</span></span>|
|<span data-ttu-id="df79c-141">email</span><span class="sxs-lookup"><span data-stu-id="df79c-141">email</span></span>|<span data-ttu-id="df79c-142">string</span><span class="sxs-lookup"><span data-stu-id="df79c-142">string</span></span>|<span data-ttu-id="df79c-143">Адрес электронной почты поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-143">The vendor's email address.</span></span>|
|<span data-ttu-id="df79c-144">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="df79c-144">website</span></span>|<span data-ttu-id="df79c-145">string</span><span class="sxs-lookup"><span data-stu-id="df79c-145">string</span></span>|<span data-ttu-id="df79c-146">Адрес веб-сайта поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-146">The vendor's website address.</span></span>|
|<span data-ttu-id="df79c-147">Таксрегистратионнумбер</span><span class="sxs-lookup"><span data-stu-id="df79c-147">taxRegistrationNumber</span></span>|<span data-ttu-id="df79c-148">string</span><span class="sxs-lookup"><span data-stu-id="df79c-148">string</span></span>|<span data-ttu-id="df79c-149">Регистрационный номер налогоплательщика поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-149">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="df79c-150">Курренциид</span><span class="sxs-lookup"><span data-stu-id="df79c-150">currencyId</span></span>|<span data-ttu-id="df79c-151">GUID</span><span class="sxs-lookup"><span data-stu-id="df79c-151">GUID</span></span>|<span data-ttu-id="df79c-152">Идентификатор кода валюты по умолчанию для поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-152">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="df79c-153">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="df79c-153">currencyCode</span></span>|<span data-ttu-id="df79c-154">string</span><span class="sxs-lookup"><span data-stu-id="df79c-154">string</span></span>|<span data-ttu-id="df79c-155">Код валюты по умолчанию для поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-155">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="df79c-156">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="df79c-156">irs1099Code</span></span>|<span data-ttu-id="df79c-157">string</span><span class="sxs-lookup"><span data-stu-id="df79c-157">string</span></span>|<span data-ttu-id="df79c-158">Указывает код 1099 для поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-158">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="df79c-159">Только для США.</span><span class="sxs-lookup"><span data-stu-id="df79c-159">US only.</span></span>|
|<span data-ttu-id="df79c-160">Пайменттермсид</span><span class="sxs-lookup"><span data-stu-id="df79c-160">paymentTermsId</span></span>|<span data-ttu-id="df79c-161">GUID</span><span class="sxs-lookup"><span data-stu-id="df79c-161">GUID</span></span>|<span data-ttu-id="df79c-162">КОД условий оплаты для поставщика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="df79c-162">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="df79c-163">Пайментмесодид</span><span class="sxs-lookup"><span data-stu-id="df79c-163">paymentMethodId</span></span>|<span data-ttu-id="df79c-164">GUID</span><span class="sxs-lookup"><span data-stu-id="df79c-164">GUID</span></span>|<span data-ttu-id="df79c-165">Идентификатор метода оплаты по умолчанию для поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-165">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="df79c-166">Такслиабле</span><span class="sxs-lookup"><span data-stu-id="df79c-166">taxLiable</span></span>|<span data-ttu-id="df79c-167">boolean</span><span class="sxs-lookup"><span data-stu-id="df79c-167">boolean</span></span>|<span data-ttu-id="df79c-168">Указывает, является ли поставщик подлежащей налогообложению.</span><span class="sxs-lookup"><span data-stu-id="df79c-168">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="df79c-169">заблокированных</span><span class="sxs-lookup"><span data-stu-id="df79c-169">blocked</span></span>|<span data-ttu-id="df79c-170">string</span><span class="sxs-lookup"><span data-stu-id="df79c-170">string</span></span>|<span data-ttu-id="df79c-171">Указывает, какие транзакции у поставщика, который не может быть разнесен.</span><span class="sxs-lookup"><span data-stu-id="df79c-171">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="df79c-172">Допустимые значения: пусто, оплата или все</span><span class="sxs-lookup"><span data-stu-id="df79c-172">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="df79c-173">равномерно</span><span class="sxs-lookup"><span data-stu-id="df79c-173">balance</span></span>|<span data-ttu-id="df79c-174">числе</span><span class="sxs-lookup"><span data-stu-id="df79c-174">decimal</span></span>|<span data-ttu-id="df79c-175">Сальдо поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-175">The vendor's balance.</span></span> <span data-ttu-id="df79c-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="df79c-176">Read-Only.</span></span>|
|<span data-ttu-id="df79c-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df79c-177">lastModifiedDateTime</span></span>|<span data-ttu-id="df79c-178">отличным</span><span class="sxs-lookup"><span data-stu-id="df79c-178">datetime</span></span>|<span data-ttu-id="df79c-179">Дата и время последнего изменения поставщика.</span><span class="sxs-lookup"><span data-stu-id="df79c-179">The last datetime the vendor was modified.</span></span> <span data-ttu-id="df79c-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="df79c-180">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="df79c-181">Отношения</span><span class="sxs-lookup"><span data-stu-id="df79c-181">Relationships</span></span>
<span data-ttu-id="df79c-182">Нет</span><span class="sxs-lookup"><span data-stu-id="df79c-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df79c-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df79c-183">JSON representation</span></span>

<span data-ttu-id="df79c-184">Ниже показано представление поставщика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df79c-184">Here is a JSON representation of the vendor.</span></span>

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

