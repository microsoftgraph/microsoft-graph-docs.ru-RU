---
title: Тип ресурса Пайментмесодс
description: Объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d72ac6ec655e15ad6f3c824dc2d5e9c3e09db0c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503651"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="de933-103">Тип ресурса Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="de933-103">paymentMethods resource type</span></span>

<span data-ttu-id="de933-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="de933-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de933-105">Представляет способ оплаты в Dynamics 365 Business Central, например PayPal, кредитную карту и банковский счет.</span><span class="sxs-lookup"><span data-stu-id="de933-105">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="de933-106">Методы</span><span class="sxs-lookup"><span data-stu-id="de933-106">Methods</span></span>

| <span data-ttu-id="de933-107">Метод</span><span class="sxs-lookup"><span data-stu-id="de933-107">Method</span></span>                                                          | <span data-ttu-id="de933-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="de933-108">Return Type</span></span>  |<span data-ttu-id="de933-109">Описание</span><span class="sxs-lookup"><span data-stu-id="de933-109">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="de933-110">Получение Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="de933-110">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="de933-111">пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="de933-111">paymentMethods</span></span>|<span data-ttu-id="de933-112">Возвращает объект метода платежа.</span><span class="sxs-lookup"><span data-stu-id="de933-112">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="de933-113">POST Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="de933-113">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="de933-114">пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="de933-114">paymentMethods</span></span>|<span data-ttu-id="de933-115">Создает объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="de933-115">Creates a payment method object.</span></span>|
|[<span data-ttu-id="de933-116">Исправление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="de933-116">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="de933-117">пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="de933-117">paymentMethods</span></span>|<span data-ttu-id="de933-118">Обновляет объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="de933-118">Updates a payment method object.</span></span>|
|[<span data-ttu-id="de933-119">Удаление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="de933-119">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="de933-120">нет</span><span class="sxs-lookup"><span data-stu-id="de933-120">none</span></span>          |<span data-ttu-id="de933-121">Удаляет объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="de933-121">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de933-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="de933-122">Properties</span></span>
| <span data-ttu-id="de933-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="de933-123">Property</span></span>           | <span data-ttu-id="de933-124">Тип</span><span class="sxs-lookup"><span data-stu-id="de933-124">Type</span></span>   |<span data-ttu-id="de933-125">Описание</span><span class="sxs-lookup"><span data-stu-id="de933-125">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="de933-126">id</span><span class="sxs-lookup"><span data-stu-id="de933-126">id</span></span>                  |<span data-ttu-id="de933-127">GUID</span><span class="sxs-lookup"><span data-stu-id="de933-127">GUID</span></span>    |<span data-ttu-id="de933-128">Уникальный идентификатор Пайментмесодс.</span><span class="sxs-lookup"><span data-stu-id="de933-128">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="de933-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="de933-129">Non-editable.</span></span>           |
|<span data-ttu-id="de933-130">code</span><span class="sxs-lookup"><span data-stu-id="de933-130">code</span></span>                |<span data-ttu-id="de933-131">string</span><span class="sxs-lookup"><span data-stu-id="de933-131">string</span></span>  |<span data-ttu-id="de933-132">Указывает код метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="de933-132">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="de933-133">displayName</span><span class="sxs-lookup"><span data-stu-id="de933-133">displayName</span></span>         |<span data-ttu-id="de933-134">string</span><span class="sxs-lookup"><span data-stu-id="de933-134">string</span></span>  |<span data-ttu-id="de933-135">Задает отображаемое имя метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="de933-135">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="de933-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de933-136">lastModifiedDateTime</span></span>|<span data-ttu-id="de933-137">datetime</span><span class="sxs-lookup"><span data-stu-id="de933-137">datetime</span></span>|<span data-ttu-id="de933-138">Дата и время последнего изменения метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="de933-138">The last datetime the payment method was modified.</span></span> <span data-ttu-id="de933-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="de933-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="de933-140">Связи</span><span class="sxs-lookup"><span data-stu-id="de933-140">Relationships</span></span>
<span data-ttu-id="de933-141">Нет</span><span class="sxs-lookup"><span data-stu-id="de933-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de933-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de933-142">JSON representation</span></span>

<span data-ttu-id="de933-143">Ниже показано представление объекта Пайментмесодс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de933-143">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
