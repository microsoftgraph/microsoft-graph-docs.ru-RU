---
title: Тип ресурса Компанинформатион
description: Сведения о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ce982e7d03e4b2e5947381173d57706f6cf8f41e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505128"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="462e6-103">Тип ресурса Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="462e6-103">companyInformation resource type</span></span>

<span data-ttu-id="462e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="462e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="462e6-105">Представляет сведения, указанные для текущей компании в Dynamics 365 Business Central, такие как имя, адрес, адрес электронной почты и адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="462e6-105">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="462e6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="462e6-106">Methods</span></span>

| <span data-ttu-id="462e6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="462e6-107">Method</span></span>         | <span data-ttu-id="462e6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="462e6-108">Return Type</span></span>  |<span data-ttu-id="462e6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="462e6-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="462e6-110">Получение Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="462e6-110">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="462e6-111">компанинформатион</span><span class="sxs-lookup"><span data-stu-id="462e6-111">companyInformation</span></span>|<span data-ttu-id="462e6-112">Получает сведения о компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-112">Gets a company information.</span></span>|
|[<span data-ttu-id="462e6-113">Исправление Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="462e6-113">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="462e6-114">компанинформатион</span><span class="sxs-lookup"><span data-stu-id="462e6-114">companyInformation</span></span>|<span data-ttu-id="462e6-115">Обновляет сведения о компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-115">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="462e6-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="462e6-116">Properties</span></span>
| <span data-ttu-id="462e6-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="462e6-117">Property</span></span>     | <span data-ttu-id="462e6-118">Тип</span><span class="sxs-lookup"><span data-stu-id="462e6-118">Type</span></span>      |<span data-ttu-id="462e6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="462e6-119">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="462e6-120">id</span><span class="sxs-lookup"><span data-stu-id="462e6-120">id</span></span>            |<span data-ttu-id="462e6-121">GUID</span><span class="sxs-lookup"><span data-stu-id="462e6-121">GUID</span></span>|<span data-ttu-id="462e6-122">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-122">The unique ID of the company.</span></span> <span data-ttu-id="462e6-123">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="462e6-123">Non-editable.</span></span>|
|<span data-ttu-id="462e6-124">displayName</span><span class="sxs-lookup"><span data-stu-id="462e6-124">displayName</span></span>   |<span data-ttu-id="462e6-125">string</span><span class="sxs-lookup"><span data-stu-id="462e6-125">string</span></span>   |<span data-ttu-id="462e6-126">Отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-126">The company's display name.</span></span>           |
|<span data-ttu-id="462e6-127">address</span><span class="sxs-lookup"><span data-stu-id="462e6-127">address</span></span>       |[<span data-ttu-id="462e6-128">Навигационная. посталаддресс</span><span class="sxs-lookup"><span data-stu-id="462e6-128">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="462e6-129">Адрес компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-129">The company's address.</span></span> <span data-ttu-id="462e6-130">Просмотрите сложный тип для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="462e6-130">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="462e6-131">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="462e6-131">phoneNumber</span></span>   |<span data-ttu-id="462e6-132">string</span><span class="sxs-lookup"><span data-stu-id="462e6-132">string</span></span>   |<span data-ttu-id="462e6-133">Номер телефона компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-133">The company's telephone number.</span></span>       |
|<span data-ttu-id="462e6-134">faxNumber</span><span class="sxs-lookup"><span data-stu-id="462e6-134">faxNumber</span></span>     |<span data-ttu-id="462e6-135">string</span><span class="sxs-lookup"><span data-stu-id="462e6-135">string</span></span>   |<span data-ttu-id="462e6-136">Номер факса компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-136">The company's fax number.</span></span>             |
|<span data-ttu-id="462e6-137">email</span><span class="sxs-lookup"><span data-stu-id="462e6-137">email</span></span>         |<span data-ttu-id="462e6-138">строка</span><span class="sxs-lookup"><span data-stu-id="462e6-138">string</span></span>   |<span data-ttu-id="462e6-139">Адрес электронной почты компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-139">The company's email address.</span></span>          |
|<span data-ttu-id="462e6-140">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="462e6-140">website</span></span>       |<span data-ttu-id="462e6-141">string</span><span class="sxs-lookup"><span data-stu-id="462e6-141">string</span></span>   |<span data-ttu-id="462e6-142">Адрес веб-сайта компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-142">The company's website address.</span></span>        |
|<span data-ttu-id="462e6-143">таксрегистратионнумбер</span><span class="sxs-lookup"><span data-stu-id="462e6-143">taxRegistrationNumber</span></span>|<span data-ttu-id="462e6-144">string</span><span class="sxs-lookup"><span data-stu-id="462e6-144">string</span></span>|<span data-ttu-id="462e6-145">Регистрационный номер налогоплательщика компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-145">The company's tax registration number.</span></span>|
|<span data-ttu-id="462e6-146">курренцикоде</span><span class="sxs-lookup"><span data-stu-id="462e6-146">currencyCode</span></span>  |<span data-ttu-id="462e6-147">string</span><span class="sxs-lookup"><span data-stu-id="462e6-147">string</span></span>   |<span data-ttu-id="462e6-148">Валюта, в которой компания выполняет бизнес.</span><span class="sxs-lookup"><span data-stu-id="462e6-148">The currency the company does business in.</span></span> <span data-ttu-id="462e6-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="462e6-149">Read-Only.</span></span>|
|<span data-ttu-id="462e6-150">куррентфискалеарстартдате</span><span class="sxs-lookup"><span data-stu-id="462e6-150">currentFiscalYearStartDate</span></span>|<span data-ttu-id="462e6-151">date</span><span class="sxs-lookup"><span data-stu-id="462e6-151">date</span></span>|<span data-ttu-id="462e6-152">Текущая дата начала финансового года компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-152">The company's current fiscal year start date.</span></span> <span data-ttu-id="462e6-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="462e6-153">Read-Only.</span></span>|
|<span data-ttu-id="462e6-154">источников</span><span class="sxs-lookup"><span data-stu-id="462e6-154">industry</span></span>      |<span data-ttu-id="462e6-155">string</span><span class="sxs-lookup"><span data-stu-id="462e6-155">string</span></span>   |<span data-ttu-id="462e6-156">Отрасль, в которой участвует компания.</span><span class="sxs-lookup"><span data-stu-id="462e6-156">The industry the company is part of.</span></span>  |
|<span data-ttu-id="462e6-157">графические</span><span class="sxs-lookup"><span data-stu-id="462e6-157">picture</span></span>       |<span data-ttu-id="462e6-158">stream</span><span class="sxs-lookup"><span data-stu-id="462e6-158">stream</span></span>   |<span data-ttu-id="462e6-159">Логотип компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-159">The company logo.</span></span> <span data-ttu-id="462e6-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="462e6-160">Read-Only.</span></span>          |
|<span data-ttu-id="462e6-161">бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="462e6-161">businessProfileId</span></span>|<span data-ttu-id="462e6-162">string</span><span class="sxs-lookup"><span data-stu-id="462e6-162">string</span></span>|<span data-ttu-id="462e6-163">Идентификатор бизнес-профиля, связанный с компанией "Финансы".</span><span class="sxs-lookup"><span data-stu-id="462e6-163">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="462e6-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="462e6-164">Read-Only.</span></span>|
|<span data-ttu-id="462e6-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="462e6-165">lastModifiedDateTime</span></span>|<span data-ttu-id="462e6-166">datetime</span><span class="sxs-lookup"><span data-stu-id="462e6-166">datetime</span></span>|<span data-ttu-id="462e6-167">Дата и время последнего изменения компании.</span><span class="sxs-lookup"><span data-stu-id="462e6-167">The last datetime the company was modified.</span></span> <span data-ttu-id="462e6-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="462e6-168">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="462e6-169">Связи</span><span class="sxs-lookup"><span data-stu-id="462e6-169">Relationships</span></span>
<span data-ttu-id="462e6-170">Нет</span><span class="sxs-lookup"><span data-stu-id="462e6-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="462e6-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="462e6-171">JSON representation</span></span>

<span data-ttu-id="462e6-172">Ниже представлено представление объекта Компанинформатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="462e6-172">Here is a JSON representation of the companyInformation</span></span>
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

