---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 6720a8959ddba79d1face9c91325900c3a35a95c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973732"
---
# <a name="companies-resource-type"></a><span data-ttu-id="30fb4-103">Тип ресурса "компании"</span><span class="sxs-lookup"><span data-stu-id="30fb4-103">companies resource type</span></span>
<span data-ttu-id="30fb4-104">Представляет тип ресурса "компании" в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="30fb4-104">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="30fb4-105">Методы</span><span class="sxs-lookup"><span data-stu-id="30fb4-105">Methods</span></span>

| <span data-ttu-id="30fb4-106">Метод</span><span class="sxs-lookup"><span data-stu-id="30fb4-106">Method</span></span>         | <span data-ttu-id="30fb4-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="30fb4-107">Return Type</span></span>  |<span data-ttu-id="30fb4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="30fb4-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="30fb4-109">Получение компаний</span><span class="sxs-lookup"><span data-stu-id="30fb4-109">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="30fb4-110">companies</span><span class="sxs-lookup"><span data-stu-id="30fb4-110">companies</span></span>|<span data-ttu-id="30fb4-111">Получение компании.</span><span class="sxs-lookup"><span data-stu-id="30fb4-111">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="30fb4-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="30fb4-112">Properties</span></span>
| <span data-ttu-id="30fb4-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="30fb4-113">Property</span></span>        | <span data-ttu-id="30fb4-114">Тип</span><span class="sxs-lookup"><span data-stu-id="30fb4-114">Type</span></span> |<span data-ttu-id="30fb4-115">Описание</span><span class="sxs-lookup"><span data-stu-id="30fb4-115">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="30fb4-116">id</span><span class="sxs-lookup"><span data-stu-id="30fb4-116">id</span></span>               |<span data-ttu-id="30fb4-117">GUID</span><span class="sxs-lookup"><span data-stu-id="30fb4-117">GUID</span></span>  |<span data-ttu-id="30fb4-118">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="30fb4-118">The unique ID of the company.</span></span> <span data-ttu-id="30fb4-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30fb4-119">Read-Only.</span></span>|
|<span data-ttu-id="30fb4-120">name</span><span class="sxs-lookup"><span data-stu-id="30fb4-120">name</span></span>             |<span data-ttu-id="30fb4-121">string</span><span class="sxs-lookup"><span data-stu-id="30fb4-121">string</span></span>|<span data-ttu-id="30fb4-122">Указывает компанию.</span><span class="sxs-lookup"><span data-stu-id="30fb4-122">Specifies the Company.</span></span>                  |
|<span data-ttu-id="30fb4-123">displayName</span><span class="sxs-lookup"><span data-stu-id="30fb4-123">displayName</span></span>      |<span data-ttu-id="30fb4-124">string</span><span class="sxs-lookup"><span data-stu-id="30fb4-124">string</span></span>|<span data-ttu-id="30fb4-125">Задает отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="30fb4-125">Specifies the company display name.</span></span>     |
|<span data-ttu-id="30fb4-126">Системверсион</span><span class="sxs-lookup"><span data-stu-id="30fb4-126">systemVersion</span></span>    |<span data-ttu-id="30fb4-127">string</span><span class="sxs-lookup"><span data-stu-id="30fb4-127">string</span></span>|<span data-ttu-id="30fb4-128">Указывает внутреннюю версию компании.</span><span class="sxs-lookup"><span data-stu-id="30fb4-128">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="30fb4-129">Бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="30fb4-129">businessProfileId</span></span>|<span data-ttu-id="30fb4-130">string</span><span class="sxs-lookup"><span data-stu-id="30fb4-130">string</span></span>|<span data-ttu-id="30fb4-131">Указывает идентификатор бизнес-профиля, связанный с компанией.</span><span class="sxs-lookup"><span data-stu-id="30fb4-131">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="30fb4-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="30fb4-132">Relationships</span></span>
<span data-ttu-id="30fb4-133">Нет</span><span class="sxs-lookup"><span data-stu-id="30fb4-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30fb4-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30fb4-134">JSON representation</span></span>

<span data-ttu-id="30fb4-135">Ниже показано представление компании в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30fb4-135">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


