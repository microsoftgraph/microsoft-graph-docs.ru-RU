---
title: Тип ресурса Компанинформатион
description: Сведения о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0f8671cbade11cc9db6bf797c39eb17acf286ef7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507275"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="efa9e-103">Тип ресурса Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="efa9e-103">companyInformation resource type</span></span>
<span data-ttu-id="efa9e-104">Представляет сведения, указанные для текущей компании в Dynamics 365 Business Central, такие как имя, адрес, адрес электронной почты и адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="efa9e-104">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="efa9e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="efa9e-105">Methods</span></span>

| <span data-ttu-id="efa9e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="efa9e-106">Method</span></span>         | <span data-ttu-id="efa9e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="efa9e-107">Return Type</span></span>  |<span data-ttu-id="efa9e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="efa9e-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="efa9e-109">Получение Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="efa9e-109">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="efa9e-110">Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="efa9e-110">companyInformation</span></span>|<span data-ttu-id="efa9e-111">Получает сведения о компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-111">Gets a company information.</span></span>|
|[<span data-ttu-id="efa9e-112">Исправление Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="efa9e-112">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="efa9e-113">Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="efa9e-113">companyInformation</span></span>|<span data-ttu-id="efa9e-114">Обновляет сведения о компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-114">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="efa9e-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="efa9e-115">Properties</span></span>
| <span data-ttu-id="efa9e-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa9e-116">Property</span></span>     | <span data-ttu-id="efa9e-117">Тип</span><span class="sxs-lookup"><span data-stu-id="efa9e-117">Type</span></span>      |<span data-ttu-id="efa9e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="efa9e-118">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="efa9e-119">id</span><span class="sxs-lookup"><span data-stu-id="efa9e-119">id</span></span>            |<span data-ttu-id="efa9e-120">GUID</span><span class="sxs-lookup"><span data-stu-id="efa9e-120">GUID</span></span>|<span data-ttu-id="efa9e-121">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-121">The unique ID of the company.</span></span> <span data-ttu-id="efa9e-122">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="efa9e-122">Non-editable.</span></span>|
|<span data-ttu-id="efa9e-123">displayName</span><span class="sxs-lookup"><span data-stu-id="efa9e-123">displayName</span></span>   |<span data-ttu-id="efa9e-124">string</span><span class="sxs-lookup"><span data-stu-id="efa9e-124">string</span></span>   |<span data-ttu-id="efa9e-125">Отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-125">The company's display name.</span></span>           |
|<span data-ttu-id="efa9e-126">address</span><span class="sxs-lookup"><span data-stu-id="efa9e-126">address</span></span>       |[<span data-ttu-id="efa9e-127">Навигационная. Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="efa9e-127">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="efa9e-128">Адрес компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-128">The company's address.</span></span> <span data-ttu-id="efa9e-129">Просмотрите сложный тип для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="efa9e-129">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="efa9e-130">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="efa9e-130">phoneNumber</span></span>   |<span data-ttu-id="efa9e-131">строка</span><span class="sxs-lookup"><span data-stu-id="efa9e-131">string</span></span>   |<span data-ttu-id="efa9e-132">Номер телефона компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-132">The company's telephone number.</span></span>       |
|<span data-ttu-id="efa9e-133">faxNumber</span><span class="sxs-lookup"><span data-stu-id="efa9e-133">faxNumber</span></span>     |<span data-ttu-id="efa9e-134">строка</span><span class="sxs-lookup"><span data-stu-id="efa9e-134">string</span></span>   |<span data-ttu-id="efa9e-135">Номер факса компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-135">The company's fax number.</span></span>             |
|<span data-ttu-id="efa9e-136">email</span><span class="sxs-lookup"><span data-stu-id="efa9e-136">email</span></span>         |<span data-ttu-id="efa9e-137">строка</span><span class="sxs-lookup"><span data-stu-id="efa9e-137">string</span></span>   |<span data-ttu-id="efa9e-138">Адрес электронной почты компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-138">The company's email address.</span></span>          |
|<span data-ttu-id="efa9e-139">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="efa9e-139">website</span></span>       |<span data-ttu-id="efa9e-140">строка</span><span class="sxs-lookup"><span data-stu-id="efa9e-140">string</span></span>   |<span data-ttu-id="efa9e-141">Адрес веб-сайта компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-141">The company's website address.</span></span>        |
|<span data-ttu-id="efa9e-142">Таксрегистратионнумбер</span><span class="sxs-lookup"><span data-stu-id="efa9e-142">taxRegistrationNumber</span></span>|<span data-ttu-id="efa9e-143">строка</span><span class="sxs-lookup"><span data-stu-id="efa9e-143">string</span></span>|<span data-ttu-id="efa9e-144">Регистрационный номер налогоплательщика компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-144">The company's tax registration number.</span></span>|
|<span data-ttu-id="efa9e-145">Курренцикоде</span><span class="sxs-lookup"><span data-stu-id="efa9e-145">currencyCode</span></span>  |<span data-ttu-id="efa9e-146">строка</span><span class="sxs-lookup"><span data-stu-id="efa9e-146">string</span></span>   |<span data-ttu-id="efa9e-147">Валюта, в которой компания выполняет бизнес.</span><span class="sxs-lookup"><span data-stu-id="efa9e-147">The currency the company does business in.</span></span> <span data-ttu-id="efa9e-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efa9e-148">Read-Only.</span></span>|
|<span data-ttu-id="efa9e-149">Куррентфискалеарстартдате</span><span class="sxs-lookup"><span data-stu-id="efa9e-149">currentFiscalYearStartDate</span></span>|<span data-ttu-id="efa9e-150">дата</span><span class="sxs-lookup"><span data-stu-id="efa9e-150">date</span></span>|<span data-ttu-id="efa9e-151">Текущая дата начала финансового года компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-151">The company's current fiscal year start date.</span></span> <span data-ttu-id="efa9e-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efa9e-152">Read-Only.</span></span>|
|<span data-ttu-id="efa9e-153">источников</span><span class="sxs-lookup"><span data-stu-id="efa9e-153">industry</span></span>      |<span data-ttu-id="efa9e-154">строка</span><span class="sxs-lookup"><span data-stu-id="efa9e-154">string</span></span>   |<span data-ttu-id="efa9e-155">Отрасль, в которой участвует компания.</span><span class="sxs-lookup"><span data-stu-id="efa9e-155">The industry the company is part of.</span></span>  |
|<span data-ttu-id="efa9e-156">графические</span><span class="sxs-lookup"><span data-stu-id="efa9e-156">picture</span></span>       |<span data-ttu-id="efa9e-157">stream</span><span class="sxs-lookup"><span data-stu-id="efa9e-157">stream</span></span>   |<span data-ttu-id="efa9e-158">Логотип компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-158">The company logo.</span></span> <span data-ttu-id="efa9e-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efa9e-159">Read-Only.</span></span>          |
|<span data-ttu-id="efa9e-160">Бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="efa9e-160">businessProfileId</span></span>|<span data-ttu-id="efa9e-161">строка</span><span class="sxs-lookup"><span data-stu-id="efa9e-161">string</span></span>|<span data-ttu-id="efa9e-162">Идентификатор бизнес-профиля, связанный с компанией "Финансы".</span><span class="sxs-lookup"><span data-stu-id="efa9e-162">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="efa9e-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efa9e-163">Read-Only.</span></span>|
|<span data-ttu-id="efa9e-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efa9e-164">lastModifiedDateTime</span></span>|<span data-ttu-id="efa9e-165">отличным</span><span class="sxs-lookup"><span data-stu-id="efa9e-165">datetime</span></span>|<span data-ttu-id="efa9e-166">Дата и время последнего изменения компании.</span><span class="sxs-lookup"><span data-stu-id="efa9e-166">The last datetime the company was modified.</span></span> <span data-ttu-id="efa9e-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efa9e-167">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="efa9e-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="efa9e-168">Relationships</span></span>
<span data-ttu-id="efa9e-169">Нет</span><span class="sxs-lookup"><span data-stu-id="efa9e-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efa9e-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efa9e-170">JSON representation</span></span>

<span data-ttu-id="efa9e-171">Ниже представлено представление объекта Компанинформатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efa9e-171">Here is a JSON representation of the companyInformation</span></span>
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

