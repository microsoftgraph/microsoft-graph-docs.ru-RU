---
title: Тип ресурса Accounts
description: Объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 54cd9f43c5232778b5887f17974d4f556a1f3842
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142207"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="0fd17-103">Тип ресурса Accounts</span><span class="sxs-lookup"><span data-stu-id="0fd17-103">accounts resource type</span></span>

<span data-ttu-id="0fd17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fd17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fd17-105">Представляет объект Account в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="0fd17-105">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="0fd17-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0fd17-106">Methods</span></span>

| <span data-ttu-id="0fd17-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0fd17-107">Method</span></span>       | <span data-ttu-id="0fd17-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0fd17-108">Return Type</span></span>  |<span data-ttu-id="0fd17-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd17-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fd17-110">Получение учетных записей</span><span class="sxs-lookup"><span data-stu-id="0fd17-110">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="0fd17-111">учетные записи</span><span class="sxs-lookup"><span data-stu-id="0fd17-111">accounts</span></span>|<span data-ttu-id="0fd17-112">Получение объекта Accounts.</span><span class="sxs-lookup"><span data-stu-id="0fd17-112">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fd17-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fd17-113">Properties</span></span>
| <span data-ttu-id="0fd17-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fd17-114">Property</span></span>     | <span data-ttu-id="0fd17-115">Тип</span><span class="sxs-lookup"><span data-stu-id="0fd17-115">Type</span></span>   |<span data-ttu-id="0fd17-116">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd17-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fd17-117">id</span><span class="sxs-lookup"><span data-stu-id="0fd17-117">id</span></span>|<span data-ttu-id="0fd17-118">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="0fd17-118">GUID</span></span>|<span data-ttu-id="0fd17-119">Уникальный идентификатор учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0fd17-119">The unique ID of the account.</span></span>|
|<span data-ttu-id="0fd17-120">число</span><span class="sxs-lookup"><span data-stu-id="0fd17-120">number</span></span>|<span data-ttu-id="0fd17-121">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="0fd17-121">string, maximum size 20</span></span>|<span data-ttu-id="0fd17-122">Указывает номер финансового счета.</span><span class="sxs-lookup"><span data-stu-id="0fd17-122">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="0fd17-123">displayName</span><span class="sxs-lookup"><span data-stu-id="0fd17-123">displayName</span></span>|<span data-ttu-id="0fd17-124">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="0fd17-124">string, maximum size 50</span></span>|<span data-ttu-id="0fd17-125">Указывает имя финансового счета.</span><span class="sxs-lookup"><span data-stu-id="0fd17-125">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="0fd17-126">category</span><span class="sxs-lookup"><span data-stu-id="0fd17-126">category</span></span>|<span data-ttu-id="0fd17-127">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="0fd17-127">string, maximum size 20</span></span>|<span data-ttu-id="0fd17-128">Указывает категорию финансового счета.</span><span class="sxs-lookup"><span data-stu-id="0fd17-128">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="0fd17-129">Подкатегории</span><span class="sxs-lookup"><span data-stu-id="0fd17-129">subCategory</span></span>|<span data-ttu-id="0fd17-130">Строка, максимальный размер 80</span><span class="sxs-lookup"><span data-stu-id="0fd17-130">string, maximum size 80</span></span>|<span data-ttu-id="0fd17-131">Указывает подкатегорию категории счетов для финансового счета.</span><span class="sxs-lookup"><span data-stu-id="0fd17-131">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="0fd17-132">заблокированных</span><span class="sxs-lookup"><span data-stu-id="0fd17-132">blocked</span></span>|<span data-ttu-id="0fd17-133">boolean</span><span class="sxs-lookup"><span data-stu-id="0fd17-133">boolean</span></span>|<span data-ttu-id="0fd17-134">Указывает, что операции не могут быть учтены на финансовом счете.</span><span class="sxs-lookup"><span data-stu-id="0fd17-134">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="0fd17-135">**Значение true** указывает, что учетная запись заблокирована, а Разноска не разрешена.</span><span class="sxs-lookup"><span data-stu-id="0fd17-135">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="0fd17-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd17-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0fd17-137">datetime</span><span class="sxs-lookup"><span data-stu-id="0fd17-137">datetime</span></span>|<span data-ttu-id="0fd17-138">Дата и время последнего изменения учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0fd17-138">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="0fd17-139">Связи</span><span class="sxs-lookup"><span data-stu-id="0fd17-139">Relationships</span></span>
<span data-ttu-id="0fd17-140">Нет</span><span class="sxs-lookup"><span data-stu-id="0fd17-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fd17-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0fd17-141">JSON representation</span></span>

<span data-ttu-id="0fd17-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fd17-142">Here is a JSON representation of the resource.</span></span>


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
