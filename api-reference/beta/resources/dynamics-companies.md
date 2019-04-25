---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543110"
---
# <a name="companies-resource-type"></a><span data-ttu-id="b3492-103">Тип ресурса "компании"</span><span class="sxs-lookup"><span data-stu-id="b3492-103">companies resource type</span></span>
<span data-ttu-id="b3492-104">Представляет тип ресурса "компании" в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b3492-104">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="b3492-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b3492-105">Methods</span></span>

| <span data-ttu-id="b3492-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b3492-106">Method</span></span>         | <span data-ttu-id="b3492-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b3492-107">Return Type</span></span>  |<span data-ttu-id="b3492-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b3492-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="b3492-109">Получение компаний</span><span class="sxs-lookup"><span data-stu-id="b3492-109">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="b3492-110">companies</span><span class="sxs-lookup"><span data-stu-id="b3492-110">companies</span></span>|<span data-ttu-id="b3492-111">Получение компании.</span><span class="sxs-lookup"><span data-stu-id="b3492-111">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3492-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3492-112">Properties</span></span>
| <span data-ttu-id="b3492-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3492-113">Property</span></span>        | <span data-ttu-id="b3492-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b3492-114">Type</span></span> |<span data-ttu-id="b3492-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b3492-115">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="b3492-116">id</span><span class="sxs-lookup"><span data-stu-id="b3492-116">id</span></span>               |<span data-ttu-id="b3492-117">Глобальный уникальный идентификатор (GUID)</span><span class="sxs-lookup"><span data-stu-id="b3492-117">GUID</span></span>  |<span data-ttu-id="b3492-118">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="b3492-118">The unique ID of the company.</span></span> <span data-ttu-id="b3492-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b3492-119">Read-Only.</span></span>|
|<span data-ttu-id="b3492-120">name</span><span class="sxs-lookup"><span data-stu-id="b3492-120">name</span></span>             |<span data-ttu-id="b3492-121">string</span><span class="sxs-lookup"><span data-stu-id="b3492-121">string</span></span>|<span data-ttu-id="b3492-122">Указывает компанию.</span><span class="sxs-lookup"><span data-stu-id="b3492-122">Specifies the Company.</span></span>                  |
|<span data-ttu-id="b3492-123">displayName</span><span class="sxs-lookup"><span data-stu-id="b3492-123">displayName</span></span>      |<span data-ttu-id="b3492-124">string</span><span class="sxs-lookup"><span data-stu-id="b3492-124">string</span></span>|<span data-ttu-id="b3492-125">Задает отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="b3492-125">Specifies the company display name.</span></span>     |
|<span data-ttu-id="b3492-126">Системверсион</span><span class="sxs-lookup"><span data-stu-id="b3492-126">systemVersion</span></span>    |<span data-ttu-id="b3492-127">string</span><span class="sxs-lookup"><span data-stu-id="b3492-127">string</span></span>|<span data-ttu-id="b3492-128">Указывает внутреннюю версию компании.</span><span class="sxs-lookup"><span data-stu-id="b3492-128">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="b3492-129">Бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="b3492-129">businessProfileId</span></span>|<span data-ttu-id="b3492-130">string</span><span class="sxs-lookup"><span data-stu-id="b3492-130">string</span></span>|<span data-ttu-id="b3492-131">Указывает идентификатор бизнес-профиля, связанный с компанией.</span><span class="sxs-lookup"><span data-stu-id="b3492-131">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b3492-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="b3492-132">Relationships</span></span>
<span data-ttu-id="b3492-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b3492-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3492-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3492-134">JSON representation</span></span>

<span data-ttu-id="b3492-135">Ниже показано представление компании в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3492-135">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


