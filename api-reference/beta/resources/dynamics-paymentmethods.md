---
title: Тип ресурса Пайментмесодс
description: Объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: b30f97166625d45eba1a78342c219cbb74f42a8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013754"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="01b3c-103">Тип ресурса Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="01b3c-103">paymentMethods resource type</span></span>

<span data-ttu-id="01b3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01b3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01b3c-105">Представляет способ оплаты в Dynamics 365 Business Central, например PayPal, кредитную карту и банковский счет.</span><span class="sxs-lookup"><span data-stu-id="01b3c-105">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="01b3c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="01b3c-106">Methods</span></span>

| <span data-ttu-id="01b3c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="01b3c-107">Method</span></span>                                                          | <span data-ttu-id="01b3c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="01b3c-108">Return Type</span></span>  |<span data-ttu-id="01b3c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="01b3c-109">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="01b3c-110">Получение Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="01b3c-110">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="01b3c-111">пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="01b3c-111">paymentMethods</span></span>|<span data-ttu-id="01b3c-112">Возвращает объект метода платежа.</span><span class="sxs-lookup"><span data-stu-id="01b3c-112">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="01b3c-113">POST Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="01b3c-113">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="01b3c-114">пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="01b3c-114">paymentMethods</span></span>|<span data-ttu-id="01b3c-115">Создает объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="01b3c-115">Creates a payment method object.</span></span>|
|[<span data-ttu-id="01b3c-116">Исправление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="01b3c-116">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="01b3c-117">пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="01b3c-117">paymentMethods</span></span>|<span data-ttu-id="01b3c-118">Обновляет объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="01b3c-118">Updates a payment method object.</span></span>|
|[<span data-ttu-id="01b3c-119">Удаление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="01b3c-119">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="01b3c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="01b3c-120">none</span></span>          |<span data-ttu-id="01b3c-121">Удаляет объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="01b3c-121">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="01b3c-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="01b3c-122">Properties</span></span>
| <span data-ttu-id="01b3c-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="01b3c-123">Property</span></span>           | <span data-ttu-id="01b3c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="01b3c-124">Type</span></span>   |<span data-ttu-id="01b3c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="01b3c-125">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="01b3c-126">id</span><span class="sxs-lookup"><span data-stu-id="01b3c-126">id</span></span>                  |<span data-ttu-id="01b3c-127">GUID</span><span class="sxs-lookup"><span data-stu-id="01b3c-127">GUID</span></span>    |<span data-ttu-id="01b3c-128">Уникальный идентификатор Пайментмесодс.</span><span class="sxs-lookup"><span data-stu-id="01b3c-128">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="01b3c-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="01b3c-129">Non-editable.</span></span>           |
|<span data-ttu-id="01b3c-130">code</span><span class="sxs-lookup"><span data-stu-id="01b3c-130">code</span></span>                |<span data-ttu-id="01b3c-131">string</span><span class="sxs-lookup"><span data-stu-id="01b3c-131">string</span></span>  |<span data-ttu-id="01b3c-132">Указывает код метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="01b3c-132">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="01b3c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="01b3c-133">displayName</span></span>         |<span data-ttu-id="01b3c-134">string</span><span class="sxs-lookup"><span data-stu-id="01b3c-134">string</span></span>  |<span data-ttu-id="01b3c-135">Задает отображаемое имя метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="01b3c-135">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="01b3c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01b3c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="01b3c-137">datetime</span><span class="sxs-lookup"><span data-stu-id="01b3c-137">datetime</span></span>|<span data-ttu-id="01b3c-138">Дата и время последнего изменения метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="01b3c-138">The last datetime the payment method was modified.</span></span> <span data-ttu-id="01b3c-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01b3c-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="01b3c-140">Связи</span><span class="sxs-lookup"><span data-stu-id="01b3c-140">Relationships</span></span>
<span data-ttu-id="01b3c-141">Нет</span><span class="sxs-lookup"><span data-stu-id="01b3c-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01b3c-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01b3c-142">JSON representation</span></span>

<span data-ttu-id="01b3c-143">Ниже показано представление объекта Пайментмесодс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01b3c-143">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


