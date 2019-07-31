---
title: Тип ресурса Пайментмесодс
description: Объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 08cfc864ee670a799a5f1672fa96cf8167ef1423
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006586"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="3ad17-103">Тип ресурса Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="3ad17-103">paymentMethods resource type</span></span>
<span data-ttu-id="3ad17-104">Представляет способ оплаты в Dynamics 365 Business Central, например PayPal, кредитную карту и банковский счет.</span><span class="sxs-lookup"><span data-stu-id="3ad17-104">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="3ad17-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3ad17-105">Methods</span></span>

| <span data-ttu-id="3ad17-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3ad17-106">Method</span></span>                                                          | <span data-ttu-id="3ad17-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ad17-107">Return Type</span></span>  |<span data-ttu-id="3ad17-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3ad17-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="3ad17-109">Получение Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="3ad17-109">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="3ad17-110">Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="3ad17-110">paymentMethods</span></span>|<span data-ttu-id="3ad17-111">Возвращает объект метода платежа.</span><span class="sxs-lookup"><span data-stu-id="3ad17-111">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="3ad17-112">POST Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="3ad17-112">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="3ad17-113">Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="3ad17-113">paymentMethods</span></span>|<span data-ttu-id="3ad17-114">Создает объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="3ad17-114">Creates a payment method object.</span></span>|
|[<span data-ttu-id="3ad17-115">Исправление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="3ad17-115">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="3ad17-116">Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="3ad17-116">paymentMethods</span></span>|<span data-ttu-id="3ad17-117">Обновляет объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="3ad17-117">Updates a payment method object.</span></span>|
|[<span data-ttu-id="3ad17-118">Удаление Пайментмесодс</span><span class="sxs-lookup"><span data-stu-id="3ad17-118">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="3ad17-119">none</span><span class="sxs-lookup"><span data-stu-id="3ad17-119">none</span></span>          |<span data-ttu-id="3ad17-120">Удаляет объект метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="3ad17-120">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ad17-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ad17-121">Properties</span></span>
| <span data-ttu-id="3ad17-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ad17-122">Property</span></span>           | <span data-ttu-id="3ad17-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3ad17-123">Type</span></span>   |<span data-ttu-id="3ad17-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3ad17-124">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="3ad17-125">id</span><span class="sxs-lookup"><span data-stu-id="3ad17-125">id</span></span>                  |<span data-ttu-id="3ad17-126">GUID</span><span class="sxs-lookup"><span data-stu-id="3ad17-126">GUID</span></span>    |<span data-ttu-id="3ad17-127">Уникальный идентификатор Пайментмесодс.</span><span class="sxs-lookup"><span data-stu-id="3ad17-127">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="3ad17-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="3ad17-128">Non-editable.</span></span>           |
|<span data-ttu-id="3ad17-129">code</span><span class="sxs-lookup"><span data-stu-id="3ad17-129">code</span></span>                |<span data-ttu-id="3ad17-130">string</span><span class="sxs-lookup"><span data-stu-id="3ad17-130">string</span></span>  |<span data-ttu-id="3ad17-131">Указывает код метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="3ad17-131">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="3ad17-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3ad17-132">displayName</span></span>         |<span data-ttu-id="3ad17-133">string</span><span class="sxs-lookup"><span data-stu-id="3ad17-133">string</span></span>  |<span data-ttu-id="3ad17-134">Задает отображаемое имя метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="3ad17-134">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="3ad17-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ad17-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3ad17-136">отличным</span><span class="sxs-lookup"><span data-stu-id="3ad17-136">datetime</span></span>|<span data-ttu-id="3ad17-137">Дата и время последнего изменения метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="3ad17-137">The last datetime the payment method was modified.</span></span> <span data-ttu-id="3ad17-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ad17-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="3ad17-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ad17-139">Relationships</span></span>
<span data-ttu-id="3ad17-140">Нет</span><span class="sxs-lookup"><span data-stu-id="3ad17-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ad17-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ad17-141">JSON representation</span></span>

<span data-ttu-id="3ad17-142">Ниже показано представление объекта Пайментмесодс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ad17-142">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
