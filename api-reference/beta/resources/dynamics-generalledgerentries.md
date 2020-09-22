---
title: Тип ресурса Женералледжерентриес
description: Запись главной книги в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 354dac3ca4912231b7ced6449f61623c18dbd36d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071334"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="a84e8-103">Тип ресурса Женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="a84e8-103">generalLedgerEntries resource type</span></span>

<span data-ttu-id="a84e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a84e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a84e8-105">Представляет объект Женералледжерентри в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a84e8-105">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="a84e8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a84e8-106">Methods</span></span>

| <span data-ttu-id="a84e8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a84e8-107">Method</span></span>       | <span data-ttu-id="a84e8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a84e8-108">Return Type</span></span>  |<span data-ttu-id="a84e8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a84e8-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="a84e8-110">Получение Женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="a84e8-110">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="a84e8-111">женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="a84e8-111">generalLedgerEntries</span></span>|<span data-ttu-id="a84e8-112">Получение объекта финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-112">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a84e8-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="a84e8-113">Properties</span></span>
| <span data-ttu-id="a84e8-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="a84e8-114">Property</span></span>           | <span data-ttu-id="a84e8-115">Тип</span><span class="sxs-lookup"><span data-stu-id="a84e8-115">Type</span></span>                  |<span data-ttu-id="a84e8-116">Описание</span><span class="sxs-lookup"><span data-stu-id="a84e8-116">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="a84e8-117">id</span><span class="sxs-lookup"><span data-stu-id="a84e8-117">id</span></span>                  |<span data-ttu-id="a84e8-118">числовых</span><span class="sxs-lookup"><span data-stu-id="a84e8-118">numeric</span></span>                |<span data-ttu-id="a84e8-119">Уникальный идентификатор финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-119">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="a84e8-120">постингдате</span><span class="sxs-lookup"><span data-stu-id="a84e8-120">postingDate</span></span>         |<span data-ttu-id="a84e8-121">date</span><span class="sxs-lookup"><span data-stu-id="a84e8-121">date</span></span>                   |<span data-ttu-id="a84e8-122">Указывает дату учета финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-122">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="a84e8-123">документнумбер</span><span class="sxs-lookup"><span data-stu-id="a84e8-123">documentNumber</span></span>      |<span data-ttu-id="a84e8-124">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="a84e8-124">string, maximum size 20</span></span>|<span data-ttu-id="a84e8-125">Указывает номер документа в финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-125">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="a84e8-126">documentType</span><span class="sxs-lookup"><span data-stu-id="a84e8-126">documentType</span></span>        |<span data-ttu-id="a84e8-127">string</span><span class="sxs-lookup"><span data-stu-id="a84e8-127">string</span></span>                 |<span data-ttu-id="a84e8-128">Указывает тип документа для финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-128">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="a84e8-129">accountId</span><span class="sxs-lookup"><span data-stu-id="a84e8-129">accountId</span></span>           |<span data-ttu-id="a84e8-130">GUID</span><span class="sxs-lookup"><span data-stu-id="a84e8-130">GUID</span></span>                   |<span data-ttu-id="a84e8-131">Определяет accountId финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-131">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="a84e8-132">аккаунтнумбер</span><span class="sxs-lookup"><span data-stu-id="a84e8-132">accountNumber</span></span>       |<span data-ttu-id="a84e8-133">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="a84e8-133">string, maximum size 20</span></span>|<span data-ttu-id="a84e8-134">Указывает Аккаунтнумбер финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-134">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="a84e8-135">description</span><span class="sxs-lookup"><span data-stu-id="a84e8-135">description</span></span>         |<span data-ttu-id="a84e8-136">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="a84e8-136">string, maximum size 50</span></span>|<span data-ttu-id="a84e8-137">Задает описание финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-137">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="a84e8-138">дебитамаунт</span><span class="sxs-lookup"><span data-stu-id="a84e8-138">debitAmount</span></span>         |<span data-ttu-id="a84e8-139">числовых</span><span class="sxs-lookup"><span data-stu-id="a84e8-139">numeric</span></span>                |<span data-ttu-id="a84e8-140">Указывает Дебитамаунт финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-140">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="a84e8-141">кредитамаунт</span><span class="sxs-lookup"><span data-stu-id="a84e8-141">creditAmount</span></span>        |<span data-ttu-id="a84e8-142">числовых</span><span class="sxs-lookup"><span data-stu-id="a84e8-142">numeric</span></span>                |<span data-ttu-id="a84e8-143">Указывает Кредитамаунт финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-143">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="a84e8-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a84e8-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a84e8-145">datetime</span><span class="sxs-lookup"><span data-stu-id="a84e8-145">datetime</span></span>               |<span data-ttu-id="a84e8-146">Дата и время последнего изменения финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="a84e8-146">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a84e8-147">Отношения</span><span class="sxs-lookup"><span data-stu-id="a84e8-147">Relationships</span></span>
<span data-ttu-id="a84e8-148">Нет</span><span class="sxs-lookup"><span data-stu-id="a84e8-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a84e8-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a84e8-149">JSON representation</span></span>

<span data-ttu-id="a84e8-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a84e8-150">Here is a JSON representation of the resource.</span></span>


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



