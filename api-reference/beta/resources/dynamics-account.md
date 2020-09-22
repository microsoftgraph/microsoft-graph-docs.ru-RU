---
title: Тип ресурса Accounts
description: Объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 671d81da52b28558fa5c24b13060b766c8d908c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076458"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="0df6c-103">Тип ресурса Accounts</span><span class="sxs-lookup"><span data-stu-id="0df6c-103">accounts resource type</span></span>

<span data-ttu-id="0df6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0df6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df6c-105">Представляет объект Account в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="0df6c-105">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="0df6c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0df6c-106">Methods</span></span>

| <span data-ttu-id="0df6c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0df6c-107">Method</span></span>       | <span data-ttu-id="0df6c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0df6c-108">Return Type</span></span>  |<span data-ttu-id="0df6c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0df6c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0df6c-110">Получение учетных записей</span><span class="sxs-lookup"><span data-stu-id="0df6c-110">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="0df6c-111">учетные записи</span><span class="sxs-lookup"><span data-stu-id="0df6c-111">accounts</span></span>|<span data-ttu-id="0df6c-112">Получение объекта Accounts.</span><span class="sxs-lookup"><span data-stu-id="0df6c-112">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0df6c-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="0df6c-113">Properties</span></span>
| <span data-ttu-id="0df6c-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="0df6c-114">Property</span></span>     | <span data-ttu-id="0df6c-115">Тип</span><span class="sxs-lookup"><span data-stu-id="0df6c-115">Type</span></span>   |<span data-ttu-id="0df6c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="0df6c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0df6c-117">id</span><span class="sxs-lookup"><span data-stu-id="0df6c-117">id</span></span>|<span data-ttu-id="0df6c-118">GUID</span><span class="sxs-lookup"><span data-stu-id="0df6c-118">GUID</span></span>|<span data-ttu-id="0df6c-119">Уникальный идентификатор учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0df6c-119">The unique ID of the account.</span></span>|
|<span data-ttu-id="0df6c-120">число</span><span class="sxs-lookup"><span data-stu-id="0df6c-120">number</span></span>|<span data-ttu-id="0df6c-121">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="0df6c-121">string, maximum size 20</span></span>|<span data-ttu-id="0df6c-122">Указывает номер финансового счета.</span><span class="sxs-lookup"><span data-stu-id="0df6c-122">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="0df6c-123">displayName</span><span class="sxs-lookup"><span data-stu-id="0df6c-123">displayName</span></span>|<span data-ttu-id="0df6c-124">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="0df6c-124">string, maximum size 50</span></span>|<span data-ttu-id="0df6c-125">Указывает имя финансового счета.</span><span class="sxs-lookup"><span data-stu-id="0df6c-125">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="0df6c-126">category</span><span class="sxs-lookup"><span data-stu-id="0df6c-126">category</span></span>|<span data-ttu-id="0df6c-127">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="0df6c-127">string, maximum size 20</span></span>|<span data-ttu-id="0df6c-128">Указывает категорию финансового счета.</span><span class="sxs-lookup"><span data-stu-id="0df6c-128">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="0df6c-129">Подкатегории</span><span class="sxs-lookup"><span data-stu-id="0df6c-129">subCategory</span></span>|<span data-ttu-id="0df6c-130">Строка, максимальный размер 80</span><span class="sxs-lookup"><span data-stu-id="0df6c-130">string, maximum size 80</span></span>|<span data-ttu-id="0df6c-131">Указывает подкатегорию категории счетов для финансового счета.</span><span class="sxs-lookup"><span data-stu-id="0df6c-131">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="0df6c-132">заблокированных</span><span class="sxs-lookup"><span data-stu-id="0df6c-132">blocked</span></span>|<span data-ttu-id="0df6c-133">boolean</span><span class="sxs-lookup"><span data-stu-id="0df6c-133">boolean</span></span>|<span data-ttu-id="0df6c-134">Указывает, что операции не могут быть учтены на финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="0df6c-134">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="0df6c-135">**Значение true** указывает, что учетная запись заблокирована, а Разноска не разрешена.</span><span class="sxs-lookup"><span data-stu-id="0df6c-135">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="0df6c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0df6c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0df6c-137">datetime</span><span class="sxs-lookup"><span data-stu-id="0df6c-137">datetime</span></span>|<span data-ttu-id="0df6c-138">Дата и время последнего изменения учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0df6c-138">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="0df6c-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="0df6c-139">Relationships</span></span>
<span data-ttu-id="0df6c-140">Нет</span><span class="sxs-lookup"><span data-stu-id="0df6c-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0df6c-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0df6c-141">JSON representation</span></span>

<span data-ttu-id="0df6c-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0df6c-142">Here is a JSON representation of the resource.</span></span>


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


