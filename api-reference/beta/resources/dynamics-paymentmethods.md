---
title: Тип ресурса Пайментмесодс
description: Объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1e4cd044d4b552a9239b742efb302633524ce22b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366650"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="85d28-103">Тип ресурса Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="85d28-103">paymentMethods resource type</span></span>
<span data-ttu-id="85d28-104">Представляет способ оплаты в Dynamics 365 Business Central, например PayPal, кредитную карту и банковский счет.</span><span class="sxs-lookup"><span data-stu-id="85d28-104">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="85d28-105">Методы</span><span class="sxs-lookup"><span data-stu-id="85d28-105">Methods</span></span>

| <span data-ttu-id="85d28-106">Метод</span><span class="sxs-lookup"><span data-stu-id="85d28-106">Method</span></span>                                                          | <span data-ttu-id="85d28-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85d28-107">Return Type</span></span>  |<span data-ttu-id="85d28-108">Описание</span><span class="sxs-lookup"><span data-stu-id="85d28-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="85d28-109">Получение Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="85d28-109">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="85d28-110">Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="85d28-110">paymentMethods</span></span>|<span data-ttu-id="85d28-111">Возвращает объект метода платежа.</span><span class="sxs-lookup"><span data-stu-id="85d28-111">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="85d28-112">POST Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="85d28-112">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="85d28-113">Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="85d28-113">paymentMethods</span></span>|<span data-ttu-id="85d28-114">Создает объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="85d28-114">Creates a payment method object.</span></span>|
|[<span data-ttu-id="85d28-115">Исправление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="85d28-115">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="85d28-116">Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="85d28-116">paymentMethods</span></span>|<span data-ttu-id="85d28-117">Обновляет объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="85d28-117">Updates a payment method object.</span></span>|
|[<span data-ttu-id="85d28-118">Удаление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="85d28-118">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="85d28-119">Нет</span><span class="sxs-lookup"><span data-stu-id="85d28-119">none</span></span>          |<span data-ttu-id="85d28-120">Удаляет объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="85d28-120">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="85d28-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="85d28-121">Properties</span></span>
| <span data-ttu-id="85d28-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="85d28-122">Property</span></span>           | <span data-ttu-id="85d28-123">Тип</span><span class="sxs-lookup"><span data-stu-id="85d28-123">Type</span></span>   |<span data-ttu-id="85d28-124">Описание</span><span class="sxs-lookup"><span data-stu-id="85d28-124">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="85d28-125">id</span><span class="sxs-lookup"><span data-stu-id="85d28-125">id</span></span>                  |<span data-ttu-id="85d28-126">GUID</span><span class="sxs-lookup"><span data-stu-id="85d28-126">GUID</span></span>    |<span data-ttu-id="85d28-127">Уникальный идентификатор Пайментмесодс.</span><span class="sxs-lookup"><span data-stu-id="85d28-127">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="85d28-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="85d28-128">Non-editable.</span></span>           |
|<span data-ttu-id="85d28-129">code</span><span class="sxs-lookup"><span data-stu-id="85d28-129">code</span></span>                |<span data-ttu-id="85d28-130">строка</span><span class="sxs-lookup"><span data-stu-id="85d28-130">string</span></span>  |<span data-ttu-id="85d28-131">Указывает код метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="85d28-131">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="85d28-132">displayName</span><span class="sxs-lookup"><span data-stu-id="85d28-132">displayName</span></span>         |<span data-ttu-id="85d28-133">строка</span><span class="sxs-lookup"><span data-stu-id="85d28-133">string</span></span>  |<span data-ttu-id="85d28-134">Задает отображаемое имя метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="85d28-134">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="85d28-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85d28-135">lastModifiedDateTime</span></span>|<span data-ttu-id="85d28-136">отличным</span><span class="sxs-lookup"><span data-stu-id="85d28-136">datetime</span></span>|<span data-ttu-id="85d28-137">Дата и время последнего изменения метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="85d28-137">The last datetime the payment method was modified.</span></span> <span data-ttu-id="85d28-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85d28-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="85d28-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="85d28-139">Relationships</span></span>
<span data-ttu-id="85d28-140">Нет</span><span class="sxs-lookup"><span data-stu-id="85d28-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85d28-141">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="85d28-141">JSON representation</span></span>

<span data-ttu-id="85d28-142">Ниже показано представление объекта Пайментмесодс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85d28-142">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
