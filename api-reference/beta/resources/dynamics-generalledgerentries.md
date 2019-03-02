---
title: Тип ресурса Женералледжерентриес
description: Запись главной книги в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365761"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="07f06-103">Тип ресурса Женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="07f06-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="07f06-104">Представляет объект Женералледжерентри в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="07f06-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="07f06-105">Методы</span><span class="sxs-lookup"><span data-stu-id="07f06-105">Methods</span></span>

| <span data-ttu-id="07f06-106">Метод</span><span class="sxs-lookup"><span data-stu-id="07f06-106">Method</span></span>       | <span data-ttu-id="07f06-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="07f06-107">Return Type</span></span>  |<span data-ttu-id="07f06-108">Описание</span><span class="sxs-lookup"><span data-stu-id="07f06-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="07f06-109">Получение Женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="07f06-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="07f06-110">Женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="07f06-110">generalLedgerEntries</span></span>|<span data-ttu-id="07f06-111">Получение объекта финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07f06-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="07f06-112">Properties</span></span>
| <span data-ttu-id="07f06-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="07f06-113">Property</span></span>           | <span data-ttu-id="07f06-114">Тип</span><span class="sxs-lookup"><span data-stu-id="07f06-114">Type</span></span>                  |<span data-ttu-id="07f06-115">Описание</span><span class="sxs-lookup"><span data-stu-id="07f06-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="07f06-116">id</span><span class="sxs-lookup"><span data-stu-id="07f06-116">id</span></span>                  |<span data-ttu-id="07f06-117">числовых</span><span class="sxs-lookup"><span data-stu-id="07f06-117">numeric</span></span>                |<span data-ttu-id="07f06-118">Уникальный идентификатор финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="07f06-119">Постингдате</span><span class="sxs-lookup"><span data-stu-id="07f06-119">postingDate</span></span>         |<span data-ttu-id="07f06-120">дата</span><span class="sxs-lookup"><span data-stu-id="07f06-120">date</span></span>                   |<span data-ttu-id="07f06-121">Указывает дату учета финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="07f06-122">Документнумбер</span><span class="sxs-lookup"><span data-stu-id="07f06-122">documentNumber</span></span>      |<span data-ttu-id="07f06-123">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="07f06-123">string, maximum size 20</span></span>|<span data-ttu-id="07f06-124">Указывает номер документа в финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="07f06-125">documentType</span><span class="sxs-lookup"><span data-stu-id="07f06-125">documentType</span></span>        |<span data-ttu-id="07f06-126">строка</span><span class="sxs-lookup"><span data-stu-id="07f06-126">string</span></span>                 |<span data-ttu-id="07f06-127">Указывает тип документа для финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="07f06-128">accountId</span><span class="sxs-lookup"><span data-stu-id="07f06-128">accountId</span></span>           |<span data-ttu-id="07f06-129">GUID</span><span class="sxs-lookup"><span data-stu-id="07f06-129">GUID</span></span>                   |<span data-ttu-id="07f06-130">Определяет accountId финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="07f06-131">Аккаунтнумбер</span><span class="sxs-lookup"><span data-stu-id="07f06-131">accountNumber</span></span>       |<span data-ttu-id="07f06-132">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="07f06-132">string, maximum size 20</span></span>|<span data-ttu-id="07f06-133">Указывает Аккаунтнумбер финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="07f06-134">description</span><span class="sxs-lookup"><span data-stu-id="07f06-134">description</span></span>         |<span data-ttu-id="07f06-135">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="07f06-135">string, maximum size 50</span></span>|<span data-ttu-id="07f06-136">Задает описание финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="07f06-137">Дебитамаунт</span><span class="sxs-lookup"><span data-stu-id="07f06-137">debitAmount</span></span>         |<span data-ttu-id="07f06-138">числовых</span><span class="sxs-lookup"><span data-stu-id="07f06-138">numeric</span></span>                |<span data-ttu-id="07f06-139">Указывает Дебитамаунт финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="07f06-140">Кредитамаунт</span><span class="sxs-lookup"><span data-stu-id="07f06-140">creditAmount</span></span>        |<span data-ttu-id="07f06-141">числовых</span><span class="sxs-lookup"><span data-stu-id="07f06-141">numeric</span></span>                |<span data-ttu-id="07f06-142">Указывает Кредитамаунт финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="07f06-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07f06-143">lastModifiedDateTime</span></span>|<span data-ttu-id="07f06-144">отличным</span><span class="sxs-lookup"><span data-stu-id="07f06-144">datetime</span></span>               |<span data-ttu-id="07f06-145">Дата и время последнего изменения финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="07f06-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="07f06-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="07f06-146">Relationships</span></span>
<span data-ttu-id="07f06-147">Нет</span><span class="sxs-lookup"><span data-stu-id="07f06-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07f06-148">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="07f06-148">JSON representation</span></span>

<span data-ttu-id="07f06-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07f06-149">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

