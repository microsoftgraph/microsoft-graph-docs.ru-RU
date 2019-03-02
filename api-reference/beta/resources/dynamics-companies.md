---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365684"
---
# <a name="companies-resource-type"></a><span data-ttu-id="03447-103">Тип ресурса "компании"</span><span class="sxs-lookup"><span data-stu-id="03447-103">companies resource type</span></span>
<span data-ttu-id="03447-104">Представляет тип ресурса "компании" в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="03447-104">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="03447-105">Методы</span><span class="sxs-lookup"><span data-stu-id="03447-105">Methods</span></span>

| <span data-ttu-id="03447-106">Метод</span><span class="sxs-lookup"><span data-stu-id="03447-106">Method</span></span>         | <span data-ttu-id="03447-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="03447-107">Return Type</span></span>  |<span data-ttu-id="03447-108">Описание</span><span class="sxs-lookup"><span data-stu-id="03447-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="03447-109">Получение компаний</span><span class="sxs-lookup"><span data-stu-id="03447-109">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="03447-110">коммуналь</span><span class="sxs-lookup"><span data-stu-id="03447-110">companies</span></span>|<span data-ttu-id="03447-111">Получение компании.</span><span class="sxs-lookup"><span data-stu-id="03447-111">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="03447-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="03447-112">Properties</span></span>
| <span data-ttu-id="03447-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="03447-113">Property</span></span>        | <span data-ttu-id="03447-114">Тип</span><span class="sxs-lookup"><span data-stu-id="03447-114">Type</span></span> |<span data-ttu-id="03447-115">Описание</span><span class="sxs-lookup"><span data-stu-id="03447-115">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="03447-116">id</span><span class="sxs-lookup"><span data-stu-id="03447-116">id</span></span>               |<span data-ttu-id="03447-117">GUID</span><span class="sxs-lookup"><span data-stu-id="03447-117">GUID</span></span>  |<span data-ttu-id="03447-118">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="03447-118">The unique ID of the company.</span></span> <span data-ttu-id="03447-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03447-119">Read-Only.</span></span>|
|<span data-ttu-id="03447-120">name</span><span class="sxs-lookup"><span data-stu-id="03447-120">name</span></span>             |<span data-ttu-id="03447-121">string</span><span class="sxs-lookup"><span data-stu-id="03447-121">string</span></span>|<span data-ttu-id="03447-122">Указывает компанию.</span><span class="sxs-lookup"><span data-stu-id="03447-122">Specifies the Company.</span></span>                  |
|<span data-ttu-id="03447-123">displayName</span><span class="sxs-lookup"><span data-stu-id="03447-123">displayName</span></span>      |<span data-ttu-id="03447-124">строка</span><span class="sxs-lookup"><span data-stu-id="03447-124">string</span></span>|<span data-ttu-id="03447-125">Задает отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="03447-125">Specifies the company display name.</span></span>     |
|<span data-ttu-id="03447-126">Системверсион</span><span class="sxs-lookup"><span data-stu-id="03447-126">systemVersion</span></span>    |<span data-ttu-id="03447-127">строка</span><span class="sxs-lookup"><span data-stu-id="03447-127">string</span></span>|<span data-ttu-id="03447-128">Указывает внутреннюю версию компании.</span><span class="sxs-lookup"><span data-stu-id="03447-128">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="03447-129">Бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="03447-129">businessProfileId</span></span>|<span data-ttu-id="03447-130">строка</span><span class="sxs-lookup"><span data-stu-id="03447-130">string</span></span>|<span data-ttu-id="03447-131">Указывает идентификатор бизнес-профиля, связанный с компанией.</span><span class="sxs-lookup"><span data-stu-id="03447-131">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="03447-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="03447-132">Relationships</span></span>
<span data-ttu-id="03447-133">Нет</span><span class="sxs-lookup"><span data-stu-id="03447-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03447-134">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="03447-134">JSON representation</span></span>

<span data-ttu-id="03447-135">Ниже показано представление компании в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03447-135">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


