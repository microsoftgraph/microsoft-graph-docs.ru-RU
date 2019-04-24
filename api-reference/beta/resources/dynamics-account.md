---
title: Тип ресурса Accounts
description: Объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507576"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="d317e-103">Тип ресурса Accounts</span><span class="sxs-lookup"><span data-stu-id="d317e-103">accounts resource type</span></span>
<span data-ttu-id="d317e-104">Представляет объект Account в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="d317e-104">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="d317e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d317e-105">Methods</span></span>

| <span data-ttu-id="d317e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d317e-106">Method</span></span>       | <span data-ttu-id="d317e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d317e-107">Return Type</span></span>  |<span data-ttu-id="d317e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d317e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d317e-109">Получение учетных записей</span><span class="sxs-lookup"><span data-stu-id="d317e-109">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="d317e-110">см</span><span class="sxs-lookup"><span data-stu-id="d317e-110">accounts</span></span>|<span data-ttu-id="d317e-111">Получение объекта Accounts.</span><span class="sxs-lookup"><span data-stu-id="d317e-111">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d317e-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="d317e-112">Properties</span></span>
| <span data-ttu-id="d317e-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="d317e-113">Property</span></span>     | <span data-ttu-id="d317e-114">Тип</span><span class="sxs-lookup"><span data-stu-id="d317e-114">Type</span></span>   |<span data-ttu-id="d317e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="d317e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d317e-116">id</span><span class="sxs-lookup"><span data-stu-id="d317e-116">id</span></span>|<span data-ttu-id="d317e-117">GUID</span><span class="sxs-lookup"><span data-stu-id="d317e-117">GUID</span></span>|<span data-ttu-id="d317e-118">Уникальный идентификатор учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d317e-118">The unique ID of the account.</span></span>|
|<span data-ttu-id="d317e-119">number</span><span class="sxs-lookup"><span data-stu-id="d317e-119">number</span></span>|<span data-ttu-id="d317e-120">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="d317e-120">string, maximum size 20</span></span>|<span data-ttu-id="d317e-121">Указывает номер финансового счета.</span><span class="sxs-lookup"><span data-stu-id="d317e-121">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="d317e-122">displayName</span><span class="sxs-lookup"><span data-stu-id="d317e-122">displayName</span></span>|<span data-ttu-id="d317e-123">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="d317e-123">string, maximum size 50</span></span>|<span data-ttu-id="d317e-124">Указывает имя финансового счета.</span><span class="sxs-lookup"><span data-stu-id="d317e-124">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="d317e-125">category</span><span class="sxs-lookup"><span data-stu-id="d317e-125">category</span></span>|<span data-ttu-id="d317e-126">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="d317e-126">string, maximum size 20</span></span>|<span data-ttu-id="d317e-127">Указывает категорию финансового счета.</span><span class="sxs-lookup"><span data-stu-id="d317e-127">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="d317e-128">Подкатегории</span><span class="sxs-lookup"><span data-stu-id="d317e-128">subCategory</span></span>|<span data-ttu-id="d317e-129">Строка, максимальный размер 80</span><span class="sxs-lookup"><span data-stu-id="d317e-129">string, maximum size 80</span></span>|<span data-ttu-id="d317e-130">Указывает подкатегорию категории счетов для финансового счета.</span><span class="sxs-lookup"><span data-stu-id="d317e-130">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="d317e-131">заблокированных</span><span class="sxs-lookup"><span data-stu-id="d317e-131">blocked</span></span>|<span data-ttu-id="d317e-132">логический</span><span class="sxs-lookup"><span data-stu-id="d317e-132">boolean</span></span>|<span data-ttu-id="d317e-133">Указывает, что операции не могут быть учтены на финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="d317e-133">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="d317e-134">**Значение true** указывает, что учетная запись заблокирована, а Разноска не разрешена.</span><span class="sxs-lookup"><span data-stu-id="d317e-134">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="d317e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d317e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d317e-136">отличным</span><span class="sxs-lookup"><span data-stu-id="d317e-136">datetime</span></span>|<span data-ttu-id="d317e-137">Дата и время последнего изменения учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d317e-137">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d317e-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="d317e-138">Relationships</span></span>
<span data-ttu-id="d317e-139">Нет</span><span class="sxs-lookup"><span data-stu-id="d317e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d317e-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d317e-140">JSON representation</span></span>

<span data-ttu-id="d317e-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d317e-141">Here is a JSON representation of the resource.</span></span>


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
