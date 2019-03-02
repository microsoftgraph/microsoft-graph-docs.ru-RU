---
title: Тип ресурса Компанинформатион
description: Сведения о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0f8671cbade11cc9db6bf797c39eb17acf286ef7
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365915"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="3ef3a-103">Тип ресурса Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="3ef3a-103">companyInformation resource type</span></span>
<span data-ttu-id="3ef3a-104">Представляет сведения, указанные для текущей компании в Dynamics 365 Business Central, такие как имя, адрес, адрес электронной почты и адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-104">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="3ef3a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3ef3a-105">Methods</span></span>

| <span data-ttu-id="3ef3a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3ef3a-106">Method</span></span>         | <span data-ttu-id="3ef3a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ef3a-107">Return Type</span></span>  |<span data-ttu-id="3ef3a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3ef3a-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="3ef3a-109">Получение Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="3ef3a-109">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="3ef3a-110">Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="3ef3a-110">companyInformation</span></span>|<span data-ttu-id="3ef3a-111">Получает сведения о компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-111">Gets a company information.</span></span>|
|[<span data-ttu-id="3ef3a-112">Исправление Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="3ef3a-112">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="3ef3a-113">Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="3ef3a-113">companyInformation</span></span>|<span data-ttu-id="3ef3a-114">Обновляет сведения о компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-114">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="3ef3a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ef3a-115">Properties</span></span>
| <span data-ttu-id="3ef3a-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ef3a-116">Property</span></span>     | <span data-ttu-id="3ef3a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="3ef3a-117">Type</span></span>      |<span data-ttu-id="3ef3a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="3ef3a-118">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="3ef3a-119">id</span><span class="sxs-lookup"><span data-stu-id="3ef3a-119">id</span></span>            |<span data-ttu-id="3ef3a-120">GUID</span><span class="sxs-lookup"><span data-stu-id="3ef3a-120">GUID</span></span>|<span data-ttu-id="3ef3a-121">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-121">The unique ID of the company.</span></span> <span data-ttu-id="3ef3a-122">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-122">Non-editable.</span></span>|
|<span data-ttu-id="3ef3a-123">displayName</span><span class="sxs-lookup"><span data-stu-id="3ef3a-123">displayName</span></span>   |<span data-ttu-id="3ef3a-124">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-124">string</span></span>   |<span data-ttu-id="3ef3a-125">Отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-125">The company's display name.</span></span>           |
|<span data-ttu-id="3ef3a-126">address</span><span class="sxs-lookup"><span data-stu-id="3ef3a-126">address</span></span>       |[<span data-ttu-id="3ef3a-127">Навигационная. Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="3ef3a-127">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="3ef3a-128">Адрес компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-128">The company's address.</span></span> <span data-ttu-id="3ef3a-129">Просмотрите сложный тип для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-129">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="3ef3a-130">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="3ef3a-130">phoneNumber</span></span>   |<span data-ttu-id="3ef3a-131">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-131">string</span></span>   |<span data-ttu-id="3ef3a-132">Номер телефона компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-132">The company's telephone number.</span></span>       |
|<span data-ttu-id="3ef3a-133">faxNumber</span><span class="sxs-lookup"><span data-stu-id="3ef3a-133">faxNumber</span></span>     |<span data-ttu-id="3ef3a-134">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-134">string</span></span>   |<span data-ttu-id="3ef3a-135">Номер факса компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-135">The company's fax number.</span></span>             |
|<span data-ttu-id="3ef3a-136">email</span><span class="sxs-lookup"><span data-stu-id="3ef3a-136">email</span></span>         |<span data-ttu-id="3ef3a-137">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-137">string</span></span>   |<span data-ttu-id="3ef3a-138">Адрес электронной почты компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-138">The company's email address.</span></span>          |
|<span data-ttu-id="3ef3a-139">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="3ef3a-139">website</span></span>       |<span data-ttu-id="3ef3a-140">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-140">string</span></span>   |<span data-ttu-id="3ef3a-141">Адрес веб-сайта компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-141">The company's website address.</span></span>        |
|<span data-ttu-id="3ef3a-142">Таксрегистратионнумбер</span><span class="sxs-lookup"><span data-stu-id="3ef3a-142">taxRegistrationNumber</span></span>|<span data-ttu-id="3ef3a-143">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-143">string</span></span>|<span data-ttu-id="3ef3a-144">Регистрационный номер налогоплательщика компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-144">The company's tax registration number.</span></span>|
|<span data-ttu-id="3ef3a-145">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="3ef3a-145">currencyCode</span></span>  |<span data-ttu-id="3ef3a-146">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-146">string</span></span>   |<span data-ttu-id="3ef3a-147">Валюта, в которой компания выполняет бизнес.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-147">The currency the company does business in.</span></span> <span data-ttu-id="3ef3a-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-148">Read-Only.</span></span>|
|<span data-ttu-id="3ef3a-149">Куррентфискалеарстартдате</span><span class="sxs-lookup"><span data-stu-id="3ef3a-149">currentFiscalYearStartDate</span></span>|<span data-ttu-id="3ef3a-150">дата</span><span class="sxs-lookup"><span data-stu-id="3ef3a-150">date</span></span>|<span data-ttu-id="3ef3a-151">Текущая дата начала финансового года компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-151">The company's current fiscal year start date.</span></span> <span data-ttu-id="3ef3a-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-152">Read-Only.</span></span>|
|<span data-ttu-id="3ef3a-153">источников</span><span class="sxs-lookup"><span data-stu-id="3ef3a-153">industry</span></span>      |<span data-ttu-id="3ef3a-154">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-154">string</span></span>   |<span data-ttu-id="3ef3a-155">Отрасль, в которой участвует компания.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-155">The industry the company is part of.</span></span>  |
|<span data-ttu-id="3ef3a-156">графические</span><span class="sxs-lookup"><span data-stu-id="3ef3a-156">picture</span></span>       |<span data-ttu-id="3ef3a-157">stream</span><span class="sxs-lookup"><span data-stu-id="3ef3a-157">stream</span></span>   |<span data-ttu-id="3ef3a-158">Логотип компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-158">The company logo.</span></span> <span data-ttu-id="3ef3a-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-159">Read-Only.</span></span>          |
|<span data-ttu-id="3ef3a-160">Бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="3ef3a-160">businessProfileId</span></span>|<span data-ttu-id="3ef3a-161">строка</span><span class="sxs-lookup"><span data-stu-id="3ef3a-161">string</span></span>|<span data-ttu-id="3ef3a-162">Идентификатор бизнес-профиля, связанный с компанией "Финансы".</span><span class="sxs-lookup"><span data-stu-id="3ef3a-162">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="3ef3a-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-163">Read-Only.</span></span>|
|<span data-ttu-id="3ef3a-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ef3a-164">lastModifiedDateTime</span></span>|<span data-ttu-id="3ef3a-165">отличным</span><span class="sxs-lookup"><span data-stu-id="3ef3a-165">datetime</span></span>|<span data-ttu-id="3ef3a-166">Дата и время последнего изменения компании.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-166">The last datetime the company was modified.</span></span> <span data-ttu-id="3ef3a-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-167">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="3ef3a-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ef3a-168">Relationships</span></span>
<span data-ttu-id="3ef3a-169">Нет</span><span class="sxs-lookup"><span data-stu-id="3ef3a-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ef3a-170">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ef3a-170">JSON representation</span></span>

<span data-ttu-id="3ef3a-171">Ниже представлено представление объекта Компанинформатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ef3a-171">Here is a JSON representation of the companyInformation</span></span>
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

