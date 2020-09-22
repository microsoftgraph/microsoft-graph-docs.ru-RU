---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3fedbd9407a4124c38a6ff08a95dbf4cd22c9fe1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081766"
---
# <a name="companies-resource-type"></a><span data-ttu-id="b91d3-103">Тип ресурса "компании"</span><span class="sxs-lookup"><span data-stu-id="b91d3-103">companies resource type</span></span>

<span data-ttu-id="b91d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b91d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b91d3-105">Представляет тип ресурса "компании" в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b91d3-105">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="b91d3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b91d3-106">Methods</span></span>

| <span data-ttu-id="b91d3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b91d3-107">Method</span></span>         | <span data-ttu-id="b91d3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b91d3-108">Return Type</span></span>  |<span data-ttu-id="b91d3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b91d3-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="b91d3-110">Получение компаний</span><span class="sxs-lookup"><span data-stu-id="b91d3-110">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="b91d3-111">companies</span><span class="sxs-lookup"><span data-stu-id="b91d3-111">companies</span></span>|<span data-ttu-id="b91d3-112">Получение компании.</span><span class="sxs-lookup"><span data-stu-id="b91d3-112">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="b91d3-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="b91d3-113">Properties</span></span>
| <span data-ttu-id="b91d3-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="b91d3-114">Property</span></span>        | <span data-ttu-id="b91d3-115">Тип</span><span class="sxs-lookup"><span data-stu-id="b91d3-115">Type</span></span> |<span data-ttu-id="b91d3-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b91d3-116">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="b91d3-117">id</span><span class="sxs-lookup"><span data-stu-id="b91d3-117">id</span></span>               |<span data-ttu-id="b91d3-118">GUID</span><span class="sxs-lookup"><span data-stu-id="b91d3-118">GUID</span></span>  |<span data-ttu-id="b91d3-119">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="b91d3-119">The unique ID of the company.</span></span> <span data-ttu-id="b91d3-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b91d3-120">Read-Only.</span></span>|
|<span data-ttu-id="b91d3-121">name</span><span class="sxs-lookup"><span data-stu-id="b91d3-121">name</span></span>             |<span data-ttu-id="b91d3-122">string</span><span class="sxs-lookup"><span data-stu-id="b91d3-122">string</span></span>|<span data-ttu-id="b91d3-123">Указывает компанию.</span><span class="sxs-lookup"><span data-stu-id="b91d3-123">Specifies the Company.</span></span>                  |
|<span data-ttu-id="b91d3-124">displayName</span><span class="sxs-lookup"><span data-stu-id="b91d3-124">displayName</span></span>      |<span data-ttu-id="b91d3-125">string</span><span class="sxs-lookup"><span data-stu-id="b91d3-125">string</span></span>|<span data-ttu-id="b91d3-126">Задает отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="b91d3-126">Specifies the company display name.</span></span>     |
|<span data-ttu-id="b91d3-127">системверсион</span><span class="sxs-lookup"><span data-stu-id="b91d3-127">systemVersion</span></span>    |<span data-ttu-id="b91d3-128">string</span><span class="sxs-lookup"><span data-stu-id="b91d3-128">string</span></span>|<span data-ttu-id="b91d3-129">Указывает внутреннюю версию компании.</span><span class="sxs-lookup"><span data-stu-id="b91d3-129">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="b91d3-130">бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="b91d3-130">businessProfileId</span></span>|<span data-ttu-id="b91d3-131">string</span><span class="sxs-lookup"><span data-stu-id="b91d3-131">string</span></span>|<span data-ttu-id="b91d3-132">Указывает идентификатор бизнес-профиля, связанный с компанией.</span><span class="sxs-lookup"><span data-stu-id="b91d3-132">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b91d3-133">Связи</span><span class="sxs-lookup"><span data-stu-id="b91d3-133">Relationships</span></span>
<span data-ttu-id="b91d3-134">Нет</span><span class="sxs-lookup"><span data-stu-id="b91d3-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b91d3-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b91d3-135">JSON representation</span></span>

<span data-ttu-id="b91d3-136">Ниже показано представление компании в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b91d3-136">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```




