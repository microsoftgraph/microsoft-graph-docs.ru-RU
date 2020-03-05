---
title: Тип ресурса Женералледжерентриес
description: Запись главной книги в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f1dc4ec7bb3fa30f7dc6362c850893953c4aa6aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503987"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="25251-103">Тип ресурса Женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="25251-103">generalLedgerEntries resource type</span></span>

<span data-ttu-id="25251-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="25251-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25251-105">Представляет объект Женералледжерентри в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="25251-105">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="25251-106">Методы</span><span class="sxs-lookup"><span data-stu-id="25251-106">Methods</span></span>

| <span data-ttu-id="25251-107">Метод</span><span class="sxs-lookup"><span data-stu-id="25251-107">Method</span></span>       | <span data-ttu-id="25251-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="25251-108">Return Type</span></span>  |<span data-ttu-id="25251-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25251-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="25251-110">Получение Женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="25251-110">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="25251-111">женералледжерентриес</span><span class="sxs-lookup"><span data-stu-id="25251-111">generalLedgerEntries</span></span>|<span data-ttu-id="25251-112">Получение объекта финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-112">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="25251-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="25251-113">Properties</span></span>
| <span data-ttu-id="25251-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="25251-114">Property</span></span>           | <span data-ttu-id="25251-115">Тип</span><span class="sxs-lookup"><span data-stu-id="25251-115">Type</span></span>                  |<span data-ttu-id="25251-116">Описание</span><span class="sxs-lookup"><span data-stu-id="25251-116">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="25251-117">id</span><span class="sxs-lookup"><span data-stu-id="25251-117">id</span></span>                  |<span data-ttu-id="25251-118">числовых</span><span class="sxs-lookup"><span data-stu-id="25251-118">numeric</span></span>                |<span data-ttu-id="25251-119">Уникальный идентификатор финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-119">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="25251-120">постингдате</span><span class="sxs-lookup"><span data-stu-id="25251-120">postingDate</span></span>         |<span data-ttu-id="25251-121">date</span><span class="sxs-lookup"><span data-stu-id="25251-121">date</span></span>                   |<span data-ttu-id="25251-122">Указывает дату учета финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-122">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="25251-123">документнумбер</span><span class="sxs-lookup"><span data-stu-id="25251-123">documentNumber</span></span>      |<span data-ttu-id="25251-124">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="25251-124">string, maximum size 20</span></span>|<span data-ttu-id="25251-125">Указывает номер документа в финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-125">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="25251-126">documentType</span><span class="sxs-lookup"><span data-stu-id="25251-126">documentType</span></span>        |<span data-ttu-id="25251-127">строка</span><span class="sxs-lookup"><span data-stu-id="25251-127">string</span></span>                 |<span data-ttu-id="25251-128">Указывает тип документа для финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-128">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="25251-129">accountId</span><span class="sxs-lookup"><span data-stu-id="25251-129">accountId</span></span>           |<span data-ttu-id="25251-130">GUID</span><span class="sxs-lookup"><span data-stu-id="25251-130">GUID</span></span>                   |<span data-ttu-id="25251-131">Определяет accountId финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-131">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="25251-132">аккаунтнумбер</span><span class="sxs-lookup"><span data-stu-id="25251-132">accountNumber</span></span>       |<span data-ttu-id="25251-133">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="25251-133">string, maximum size 20</span></span>|<span data-ttu-id="25251-134">Указывает Аккаунтнумбер финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-134">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="25251-135">description</span><span class="sxs-lookup"><span data-stu-id="25251-135">description</span></span>         |<span data-ttu-id="25251-136">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="25251-136">string, maximum size 50</span></span>|<span data-ttu-id="25251-137">Задает описание финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-137">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="25251-138">дебитамаунт</span><span class="sxs-lookup"><span data-stu-id="25251-138">debitAmount</span></span>         |<span data-ttu-id="25251-139">числовых</span><span class="sxs-lookup"><span data-stu-id="25251-139">numeric</span></span>                |<span data-ttu-id="25251-140">Указывает Дебитамаунт финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-140">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="25251-141">кредитамаунт</span><span class="sxs-lookup"><span data-stu-id="25251-141">creditAmount</span></span>        |<span data-ttu-id="25251-142">числовых</span><span class="sxs-lookup"><span data-stu-id="25251-142">numeric</span></span>                |<span data-ttu-id="25251-143">Указывает Кредитамаунт финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-143">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="25251-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25251-144">lastModifiedDateTime</span></span>|<span data-ttu-id="25251-145">datetime</span><span class="sxs-lookup"><span data-stu-id="25251-145">datetime</span></span>               |<span data-ttu-id="25251-146">Дата и время последнего изменения финансовой операции.</span><span class="sxs-lookup"><span data-stu-id="25251-146">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="25251-147">Связи</span><span class="sxs-lookup"><span data-stu-id="25251-147">Relationships</span></span>
<span data-ttu-id="25251-148">Нет</span><span class="sxs-lookup"><span data-stu-id="25251-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25251-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25251-149">JSON representation</span></span>

<span data-ttu-id="25251-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25251-150">Here is a JSON representation of the resource.</span></span>


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

