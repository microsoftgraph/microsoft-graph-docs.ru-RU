---
title: Тип ресурса Accounts
description: Объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: af6c1eccfc30259f2b86fb5a65b81d95802b67f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505282"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="56795-103">Тип ресурса Accounts</span><span class="sxs-lookup"><span data-stu-id="56795-103">accounts resource type</span></span>

<span data-ttu-id="56795-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="56795-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56795-105">Представляет объект Account в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="56795-105">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="56795-106">Методы</span><span class="sxs-lookup"><span data-stu-id="56795-106">Methods</span></span>

| <span data-ttu-id="56795-107">Метод</span><span class="sxs-lookup"><span data-stu-id="56795-107">Method</span></span>       | <span data-ttu-id="56795-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="56795-108">Return Type</span></span>  |<span data-ttu-id="56795-109">Описание</span><span class="sxs-lookup"><span data-stu-id="56795-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56795-110">Получение учетных записей</span><span class="sxs-lookup"><span data-stu-id="56795-110">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="56795-111">см</span><span class="sxs-lookup"><span data-stu-id="56795-111">accounts</span></span>|<span data-ttu-id="56795-112">Получение объекта Accounts.</span><span class="sxs-lookup"><span data-stu-id="56795-112">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56795-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="56795-113">Properties</span></span>
| <span data-ttu-id="56795-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="56795-114">Property</span></span>     | <span data-ttu-id="56795-115">Тип</span><span class="sxs-lookup"><span data-stu-id="56795-115">Type</span></span>   |<span data-ttu-id="56795-116">Описание</span><span class="sxs-lookup"><span data-stu-id="56795-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56795-117">id</span><span class="sxs-lookup"><span data-stu-id="56795-117">id</span></span>|<span data-ttu-id="56795-118">GUID</span><span class="sxs-lookup"><span data-stu-id="56795-118">GUID</span></span>|<span data-ttu-id="56795-119">Уникальный идентификатор учетной записи.</span><span class="sxs-lookup"><span data-stu-id="56795-119">The unique ID of the account.</span></span>|
|<span data-ttu-id="56795-120">число</span><span class="sxs-lookup"><span data-stu-id="56795-120">number</span></span>|<span data-ttu-id="56795-121">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="56795-121">string, maximum size 20</span></span>|<span data-ttu-id="56795-122">Указывает номер финансового счета.</span><span class="sxs-lookup"><span data-stu-id="56795-122">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="56795-123">displayName</span><span class="sxs-lookup"><span data-stu-id="56795-123">displayName</span></span>|<span data-ttu-id="56795-124">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="56795-124">string, maximum size 50</span></span>|<span data-ttu-id="56795-125">Указывает имя финансового счета.</span><span class="sxs-lookup"><span data-stu-id="56795-125">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="56795-126">category</span><span class="sxs-lookup"><span data-stu-id="56795-126">category</span></span>|<span data-ttu-id="56795-127">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="56795-127">string, maximum size 20</span></span>|<span data-ttu-id="56795-128">Указывает категорию финансового счета.</span><span class="sxs-lookup"><span data-stu-id="56795-128">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="56795-129">Подкатегории</span><span class="sxs-lookup"><span data-stu-id="56795-129">subCategory</span></span>|<span data-ttu-id="56795-130">Строка, максимальный размер 80</span><span class="sxs-lookup"><span data-stu-id="56795-130">string, maximum size 80</span></span>|<span data-ttu-id="56795-131">Указывает подкатегорию категории счетов для финансового счета.</span><span class="sxs-lookup"><span data-stu-id="56795-131">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="56795-132">заблокированных</span><span class="sxs-lookup"><span data-stu-id="56795-132">blocked</span></span>|<span data-ttu-id="56795-133">boolean</span><span class="sxs-lookup"><span data-stu-id="56795-133">boolean</span></span>|<span data-ttu-id="56795-134">Указывает, что операции не могут быть учтены на финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="56795-134">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="56795-135">**Значение true** указывает, что учетная запись заблокирована, а Разноска не разрешена.</span><span class="sxs-lookup"><span data-stu-id="56795-135">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="56795-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56795-136">lastModifiedDateTime</span></span>|<span data-ttu-id="56795-137">datetime</span><span class="sxs-lookup"><span data-stu-id="56795-137">datetime</span></span>|<span data-ttu-id="56795-138">Дата и время последнего изменения учетной записи.</span><span class="sxs-lookup"><span data-stu-id="56795-138">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="56795-139">Связи</span><span class="sxs-lookup"><span data-stu-id="56795-139">Relationships</span></span>
<span data-ttu-id="56795-140">Нет</span><span class="sxs-lookup"><span data-stu-id="56795-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56795-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56795-141">JSON representation</span></span>

<span data-ttu-id="56795-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56795-142">Here is a JSON representation of the resource.</span></span>


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
