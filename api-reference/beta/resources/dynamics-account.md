---
title: Тип ресурса Accounts
description: Объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365460"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="52440-103">Тип ресурса Accounts</span><span class="sxs-lookup"><span data-stu-id="52440-103">accounts resource type</span></span>
<span data-ttu-id="52440-104">Представляет объект Account в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="52440-104">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="52440-105">Методы</span><span class="sxs-lookup"><span data-stu-id="52440-105">Methods</span></span>

| <span data-ttu-id="52440-106">Метод</span><span class="sxs-lookup"><span data-stu-id="52440-106">Method</span></span>       | <span data-ttu-id="52440-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52440-107">Return Type</span></span>  |<span data-ttu-id="52440-108">Описание</span><span class="sxs-lookup"><span data-stu-id="52440-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52440-109">Получение учетных записей</span><span class="sxs-lookup"><span data-stu-id="52440-109">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="52440-110">учетные записи</span><span class="sxs-lookup"><span data-stu-id="52440-110">accounts</span></span>|<span data-ttu-id="52440-111">Получение объекта Accounts.</span><span class="sxs-lookup"><span data-stu-id="52440-111">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="52440-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="52440-112">Properties</span></span>
| <span data-ttu-id="52440-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="52440-113">Property</span></span>     | <span data-ttu-id="52440-114">Тип</span><span class="sxs-lookup"><span data-stu-id="52440-114">Type</span></span>   |<span data-ttu-id="52440-115">Описание</span><span class="sxs-lookup"><span data-stu-id="52440-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52440-116">id</span><span class="sxs-lookup"><span data-stu-id="52440-116">id</span></span>|<span data-ttu-id="52440-117">GUID</span><span class="sxs-lookup"><span data-stu-id="52440-117">GUID</span></span>|<span data-ttu-id="52440-118">Уникальный идентификатор учетной записи.</span><span class="sxs-lookup"><span data-stu-id="52440-118">The unique ID of the account.</span></span>|
|<span data-ttu-id="52440-119">число</span><span class="sxs-lookup"><span data-stu-id="52440-119">number</span></span>|<span data-ttu-id="52440-120">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="52440-120">string, maximum size 20</span></span>|<span data-ttu-id="52440-121">Указывает номер финансового счета.</span><span class="sxs-lookup"><span data-stu-id="52440-121">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="52440-122">displayName</span><span class="sxs-lookup"><span data-stu-id="52440-122">displayName</span></span>|<span data-ttu-id="52440-123">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="52440-123">string, maximum size 50</span></span>|<span data-ttu-id="52440-124">Указывает имя финансового счета.</span><span class="sxs-lookup"><span data-stu-id="52440-124">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="52440-125">category</span><span class="sxs-lookup"><span data-stu-id="52440-125">category</span></span>|<span data-ttu-id="52440-126">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="52440-126">string, maximum size 20</span></span>|<span data-ttu-id="52440-127">Указывает категорию финансового счета.</span><span class="sxs-lookup"><span data-stu-id="52440-127">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="52440-128">Подкатегории</span><span class="sxs-lookup"><span data-stu-id="52440-128">subCategory</span></span>|<span data-ttu-id="52440-129">Строка, максимальный размер 80</span><span class="sxs-lookup"><span data-stu-id="52440-129">string, maximum size 80</span></span>|<span data-ttu-id="52440-130">Указывает подкатегорию категории счетов для финансового счета.</span><span class="sxs-lookup"><span data-stu-id="52440-130">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="52440-131">заблокировано</span><span class="sxs-lookup"><span data-stu-id="52440-131">blocked</span></span>|<span data-ttu-id="52440-132">boolean</span><span class="sxs-lookup"><span data-stu-id="52440-132">boolean</span></span>|<span data-ttu-id="52440-133">Указывает, что операции не могут быть учтены на финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="52440-133">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="52440-134">**Значение true** указывает, что учетная запись заблокирована, а Разноска не разрешена.</span><span class="sxs-lookup"><span data-stu-id="52440-134">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="52440-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52440-135">lastModifiedDateTime</span></span>|<span data-ttu-id="52440-136">отличным</span><span class="sxs-lookup"><span data-stu-id="52440-136">datetime</span></span>|<span data-ttu-id="52440-137">Дата и время последнего изменения учетной записи.</span><span class="sxs-lookup"><span data-stu-id="52440-137">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="52440-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="52440-138">Relationships</span></span>
<span data-ttu-id="52440-139">Нет</span><span class="sxs-lookup"><span data-stu-id="52440-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52440-140">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="52440-140">JSON representation</span></span>

<span data-ttu-id="52440-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52440-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
