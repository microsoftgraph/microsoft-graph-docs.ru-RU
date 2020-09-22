---
title: Тип ресурса Компанинформатион
description: Сведения о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 05a42bfb00cb56cd560151976bc8b7c7d6ed59ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081778"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="ae2ca-103">Тип ресурса Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="ae2ca-103">companyInformation resource type</span></span>

<span data-ttu-id="ae2ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae2ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae2ca-105">Представляет сведения, указанные для текущей компании в Dynamics 365 Business Central, такие как имя, адрес, адрес электронной почты и адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-105">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="ae2ca-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ae2ca-106">Methods</span></span>

| <span data-ttu-id="ae2ca-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ae2ca-107">Method</span></span>         | <span data-ttu-id="ae2ca-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ae2ca-108">Return Type</span></span>  |<span data-ttu-id="ae2ca-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ae2ca-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="ae2ca-110">Получение Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="ae2ca-110">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="ae2ca-111">компанинформатион</span><span class="sxs-lookup"><span data-stu-id="ae2ca-111">companyInformation</span></span>|<span data-ttu-id="ae2ca-112">Получает сведения о компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-112">Gets a company information.</span></span>|
|[<span data-ttu-id="ae2ca-113">Исправление Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="ae2ca-113">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="ae2ca-114">компанинформатион</span><span class="sxs-lookup"><span data-stu-id="ae2ca-114">companyInformation</span></span>|<span data-ttu-id="ae2ca-115">Обновляет сведения о компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-115">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="ae2ca-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae2ca-116">Properties</span></span>
| <span data-ttu-id="ae2ca-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae2ca-117">Property</span></span>     | <span data-ttu-id="ae2ca-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ae2ca-118">Type</span></span>      |<span data-ttu-id="ae2ca-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ae2ca-119">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="ae2ca-120">id</span><span class="sxs-lookup"><span data-stu-id="ae2ca-120">id</span></span>            |<span data-ttu-id="ae2ca-121">GUID</span><span class="sxs-lookup"><span data-stu-id="ae2ca-121">GUID</span></span>|<span data-ttu-id="ae2ca-122">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-122">The unique ID of the company.</span></span> <span data-ttu-id="ae2ca-123">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-123">Non-editable.</span></span>|
|<span data-ttu-id="ae2ca-124">displayName</span><span class="sxs-lookup"><span data-stu-id="ae2ca-124">displayName</span></span>   |<span data-ttu-id="ae2ca-125">string</span><span class="sxs-lookup"><span data-stu-id="ae2ca-125">string</span></span>   |<span data-ttu-id="ae2ca-126">Отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-126">The company's display name.</span></span>           |
|<span data-ttu-id="ae2ca-127">address</span><span class="sxs-lookup"><span data-stu-id="ae2ca-127">address</span></span>       |[<span data-ttu-id="ae2ca-128">Навигационная. посталаддресс</span><span class="sxs-lookup"><span data-stu-id="ae2ca-128">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="ae2ca-129">Адрес компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-129">The company's address.</span></span> <span data-ttu-id="ae2ca-130">Просмотрите сложный тип для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-130">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="ae2ca-131">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ae2ca-131">phoneNumber</span></span>   |<span data-ttu-id="ae2ca-132">string</span><span class="sxs-lookup"><span data-stu-id="ae2ca-132">string</span></span>   |<span data-ttu-id="ae2ca-133">Номер телефона компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-133">The company's telephone number.</span></span>       |
|<span data-ttu-id="ae2ca-134">faxNumber</span><span class="sxs-lookup"><span data-stu-id="ae2ca-134">faxNumber</span></span>     |<span data-ttu-id="ae2ca-135">string</span><span class="sxs-lookup"><span data-stu-id="ae2ca-135">string</span></span>   |<span data-ttu-id="ae2ca-136">Номер факса компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-136">The company's fax number.</span></span>             |
|<span data-ttu-id="ae2ca-137">email</span><span class="sxs-lookup"><span data-stu-id="ae2ca-137">email</span></span>         |<span data-ttu-id="ae2ca-138">строка</span><span class="sxs-lookup"><span data-stu-id="ae2ca-138">string</span></span>   |<span data-ttu-id="ae2ca-139">Адрес электронной почты компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-139">The company's email address.</span></span>          |
|<span data-ttu-id="ae2ca-140">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="ae2ca-140">website</span></span>       |<span data-ttu-id="ae2ca-141">string</span><span class="sxs-lookup"><span data-stu-id="ae2ca-141">string</span></span>   |<span data-ttu-id="ae2ca-142">Адрес веб-сайта компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-142">The company's website address.</span></span>        |
|<span data-ttu-id="ae2ca-143">таксрегистратионнумбер</span><span class="sxs-lookup"><span data-stu-id="ae2ca-143">taxRegistrationNumber</span></span>|<span data-ttu-id="ae2ca-144">string</span><span class="sxs-lookup"><span data-stu-id="ae2ca-144">string</span></span>|<span data-ttu-id="ae2ca-145">Регистрационный номер налогоплательщика компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-145">The company's tax registration number.</span></span>|
|<span data-ttu-id="ae2ca-146">курренцикоде</span><span class="sxs-lookup"><span data-stu-id="ae2ca-146">currencyCode</span></span>  |<span data-ttu-id="ae2ca-147">string</span><span class="sxs-lookup"><span data-stu-id="ae2ca-147">string</span></span>   |<span data-ttu-id="ae2ca-148">Валюта, в которой компания выполняет бизнес.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-148">The currency the company does business in.</span></span> <span data-ttu-id="ae2ca-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-149">Read-Only.</span></span>|
|<span data-ttu-id="ae2ca-150">куррентфискалеарстартдате</span><span class="sxs-lookup"><span data-stu-id="ae2ca-150">currentFiscalYearStartDate</span></span>|<span data-ttu-id="ae2ca-151">date</span><span class="sxs-lookup"><span data-stu-id="ae2ca-151">date</span></span>|<span data-ttu-id="ae2ca-152">Текущая дата начала финансового года компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-152">The company's current fiscal year start date.</span></span> <span data-ttu-id="ae2ca-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-153">Read-Only.</span></span>|
|<span data-ttu-id="ae2ca-154">источников</span><span class="sxs-lookup"><span data-stu-id="ae2ca-154">industry</span></span>      |<span data-ttu-id="ae2ca-155">string</span><span class="sxs-lookup"><span data-stu-id="ae2ca-155">string</span></span>   |<span data-ttu-id="ae2ca-156">Отрасль, в которой участвует компания.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-156">The industry the company is part of.</span></span>  |
|<span data-ttu-id="ae2ca-157">графические</span><span class="sxs-lookup"><span data-stu-id="ae2ca-157">picture</span></span>       |<span data-ttu-id="ae2ca-158">stream</span><span class="sxs-lookup"><span data-stu-id="ae2ca-158">stream</span></span>   |<span data-ttu-id="ae2ca-159">Логотип компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-159">The company logo.</span></span> <span data-ttu-id="ae2ca-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-160">Read-Only.</span></span>          |
|<span data-ttu-id="ae2ca-161">бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="ae2ca-161">businessProfileId</span></span>|<span data-ttu-id="ae2ca-162">string</span><span class="sxs-lookup"><span data-stu-id="ae2ca-162">string</span></span>|<span data-ttu-id="ae2ca-163">Идентификатор бизнес-профиля, связанный с компанией "Финансы".</span><span class="sxs-lookup"><span data-stu-id="ae2ca-163">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="ae2ca-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-164">Read-Only.</span></span>|
|<span data-ttu-id="ae2ca-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae2ca-165">lastModifiedDateTime</span></span>|<span data-ttu-id="ae2ca-166">datetime</span><span class="sxs-lookup"><span data-stu-id="ae2ca-166">datetime</span></span>|<span data-ttu-id="ae2ca-167">Дата и время последнего изменения компании.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-167">The last datetime the company was modified.</span></span> <span data-ttu-id="ae2ca-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-168">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ae2ca-169">Связи</span><span class="sxs-lookup"><span data-stu-id="ae2ca-169">Relationships</span></span>
<span data-ttu-id="ae2ca-170">Нет</span><span class="sxs-lookup"><span data-stu-id="ae2ca-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae2ca-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae2ca-171">JSON representation</span></span>

<span data-ttu-id="ae2ca-172">Ниже представлено представление объекта Компанинформатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae2ca-172">Here is a JSON representation of the companyInformation</span></span>
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```



