---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 13bc765f873bc893925ffbddc82b2f0685376cf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505142"
---
# <a name="companies-resource-type"></a><span data-ttu-id="745a4-103">Тип ресурса "компании"</span><span class="sxs-lookup"><span data-stu-id="745a4-103">companies resource type</span></span>

<span data-ttu-id="745a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="745a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="745a4-105">Представляет тип ресурса "компании" в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="745a4-105">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="745a4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="745a4-106">Methods</span></span>

| <span data-ttu-id="745a4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="745a4-107">Method</span></span>         | <span data-ttu-id="745a4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="745a4-108">Return Type</span></span>  |<span data-ttu-id="745a4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="745a4-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="745a4-110">Получение компаний</span><span class="sxs-lookup"><span data-stu-id="745a4-110">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="745a4-111">companies</span><span class="sxs-lookup"><span data-stu-id="745a4-111">companies</span></span>|<span data-ttu-id="745a4-112">Получение компании.</span><span class="sxs-lookup"><span data-stu-id="745a4-112">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="745a4-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="745a4-113">Properties</span></span>
| <span data-ttu-id="745a4-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="745a4-114">Property</span></span>        | <span data-ttu-id="745a4-115">Тип</span><span class="sxs-lookup"><span data-stu-id="745a4-115">Type</span></span> |<span data-ttu-id="745a4-116">Описание</span><span class="sxs-lookup"><span data-stu-id="745a4-116">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="745a4-117">id</span><span class="sxs-lookup"><span data-stu-id="745a4-117">id</span></span>               |<span data-ttu-id="745a4-118">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="745a4-118">GUID</span></span>  |<span data-ttu-id="745a4-119">Уникальный идентификатор компании.</span><span class="sxs-lookup"><span data-stu-id="745a4-119">The unique ID of the company.</span></span> <span data-ttu-id="745a4-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="745a4-120">Read-Only.</span></span>|
|<span data-ttu-id="745a4-121">name</span><span class="sxs-lookup"><span data-stu-id="745a4-121">name</span></span>             |<span data-ttu-id="745a4-122">string</span><span class="sxs-lookup"><span data-stu-id="745a4-122">string</span></span>|<span data-ttu-id="745a4-123">Указывает компанию.</span><span class="sxs-lookup"><span data-stu-id="745a4-123">Specifies the Company.</span></span>                  |
|<span data-ttu-id="745a4-124">displayName</span><span class="sxs-lookup"><span data-stu-id="745a4-124">displayName</span></span>      |<span data-ttu-id="745a4-125">string</span><span class="sxs-lookup"><span data-stu-id="745a4-125">string</span></span>|<span data-ttu-id="745a4-126">Задает отображаемое имя компании.</span><span class="sxs-lookup"><span data-stu-id="745a4-126">Specifies the company display name.</span></span>     |
|<span data-ttu-id="745a4-127">системверсион</span><span class="sxs-lookup"><span data-stu-id="745a4-127">systemVersion</span></span>    |<span data-ttu-id="745a4-128">string</span><span class="sxs-lookup"><span data-stu-id="745a4-128">string</span></span>|<span data-ttu-id="745a4-129">Указывает внутреннюю версию компании.</span><span class="sxs-lookup"><span data-stu-id="745a4-129">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="745a4-130">бусинесспрофилеид</span><span class="sxs-lookup"><span data-stu-id="745a4-130">businessProfileId</span></span>|<span data-ttu-id="745a4-131">string</span><span class="sxs-lookup"><span data-stu-id="745a4-131">string</span></span>|<span data-ttu-id="745a4-132">Указывает идентификатор бизнес-профиля, связанный с компанией.</span><span class="sxs-lookup"><span data-stu-id="745a4-132">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="745a4-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="745a4-133">Relationships</span></span>
<span data-ttu-id="745a4-134">Нет</span><span class="sxs-lookup"><span data-stu-id="745a4-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="745a4-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="745a4-135">JSON representation</span></span>

<span data-ttu-id="745a4-136">Ниже показано представление компании в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="745a4-136">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


