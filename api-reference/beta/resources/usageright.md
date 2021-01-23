---
title: Тип ресурса usageRight
description: Содержит сведения об usageRight, назначенного пользователем или устройством
author: jeeshnair
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dba7f25d77379d00f48a1df820865b193cc0c084
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943750"
---
# <a name="usageright-resource-type"></a><span data-ttu-id="4f843-103">Тип ресурса usageRight</span><span class="sxs-lookup"><span data-stu-id="4f843-103">usageRight resource type</span></span>

<span data-ttu-id="4f843-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f843-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f843-105">Право на использование представляет лицензию, которая есть у пользователя или устройства для сторонних программ, основанных на приложениях питания, или для подписок на устройства (только для устройств).</span><span class="sxs-lookup"><span data-stu-id="4f843-105">A usage right represents a license that a user or device has for either third party software built on power apps or for device based subscriptions (device only).</span></span>

## <a name="methods"></a><span data-ttu-id="4f843-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4f843-106">Methods</span></span>

|<span data-ttu-id="4f843-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4f843-107">Method</span></span>|<span data-ttu-id="4f843-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="4f843-108">Return type</span></span>|<span data-ttu-id="4f843-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4f843-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f843-110">Список user usageRights</span><span class="sxs-lookup"><span data-stu-id="4f843-110">List user usageRights</span></span>](../api/user-list-usagerights.md)|<span data-ttu-id="4f843-111">[Коллекция usageRight](../resources/usageright.md)</span><span class="sxs-lookup"><span data-stu-id="4f843-111">[usageRight](../resources/usageright.md) collection</span></span>|<span data-ttu-id="4f843-112">Получите список прав на использование для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f843-112">Get the list of usage rights for a user.</span></span>|
|[<span data-ttu-id="4f843-113">Список устройств usageRights</span><span class="sxs-lookup"><span data-stu-id="4f843-113">List device usageRights</span></span>](../api/device-list-usagerights.md)|<span data-ttu-id="4f843-114">[Коллекция usageRight](../resources/usageright.md)</span><span class="sxs-lookup"><span data-stu-id="4f843-114">[usageRight](../resources/usageright.md) collection</span></span>|<span data-ttu-id="4f843-115">Получите список прав на использование для устройства.</span><span class="sxs-lookup"><span data-stu-id="4f843-115">Get the list of usage rights for a device.</span></span>|

## <a name="properties"></a><span data-ttu-id="4f843-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f843-116">Properties</span></span>

|<span data-ttu-id="4f843-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f843-117">Property</span></span>|<span data-ttu-id="4f843-118">Тип</span><span class="sxs-lookup"><span data-stu-id="4f843-118">Type</span></span>|<span data-ttu-id="4f843-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4f843-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f843-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="4f843-120">catalogId</span></span>|<span data-ttu-id="4f843-121">String</span><span class="sxs-lookup"><span data-stu-id="4f843-121">String</span></span>|<span data-ttu-id="4f843-122">ИД продукта, соответствующий правом на использование.</span><span class="sxs-lookup"><span data-stu-id="4f843-122">Product id corresponding to the usage right.</span></span>|
|<span data-ttu-id="4f843-123">id</span><span class="sxs-lookup"><span data-stu-id="4f843-123">id</span></span>|<span data-ttu-id="4f843-124">String</span><span class="sxs-lookup"><span data-stu-id="4f843-124">String</span></span>|<span data-ttu-id="4f843-125">ИД права на использование.</span><span class="sxs-lookup"><span data-stu-id="4f843-125">The id of the usage right.</span></span>|
|<span data-ttu-id="4f843-126">serviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f843-126">serviceIdentifier</span></span>|<span data-ttu-id="4f843-127">String</span><span class="sxs-lookup"><span data-stu-id="4f843-127">String</span></span>|<span data-ttu-id="4f843-128">Идентификатор службы, соответствующей правом на использование.</span><span class="sxs-lookup"><span data-stu-id="4f843-128">Identifier of the service corresponding to the usage right.</span></span>|
|<span data-ttu-id="4f843-129">state</span><span class="sxs-lookup"><span data-stu-id="4f843-129">state</span></span>|<span data-ttu-id="4f843-130">usageRightState</span><span class="sxs-lookup"><span data-stu-id="4f843-130">usageRightState</span></span>|<span data-ttu-id="4f843-131">Состояние права на использование.</span><span class="sxs-lookup"><span data-stu-id="4f843-131">The state of the usage right.</span></span> <span data-ttu-id="4f843-132">Возможные значения: `active`, `inactive`, `warning`, `suspended`.</span><span class="sxs-lookup"><span data-stu-id="4f843-132">Possible values are: `active`, `inactive`, `warning`, `suspended`.</span></span>|

### <a name="usagerightstate-values"></a><span data-ttu-id="4f843-133">значения usageRightState</span><span class="sxs-lookup"><span data-stu-id="4f843-133">usageRightState values</span></span> 

| <span data-ttu-id="4f843-134">Member</span><span class="sxs-lookup"><span data-stu-id="4f843-134">Member</span></span>             |  <span data-ttu-id="4f843-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4f843-135">Description</span></span>               |
| :----------------- |  :------------------------ |
|<span data-ttu-id="4f843-136">active</span><span class="sxs-lookup"><span data-stu-id="4f843-136">active</span></span>              | <span data-ttu-id="4f843-137">Указывает, что право на использование активно и может использоваться для предоставления преимуществ.</span><span class="sxs-lookup"><span data-stu-id="4f843-137">Indicates that the usage right is active and can be used for provisioning benefits.</span></span>|
|<span data-ttu-id="4f843-138">неактивный</span><span class="sxs-lookup"><span data-stu-id="4f843-138">inactive</span></span>                | <span data-ttu-id="4f843-139">Указывает, что право на использование не является активным и не может использоваться для предоставления преимуществ.</span><span class="sxs-lookup"><span data-stu-id="4f843-139">Indicates that the usage right is not active and cannot be used for provisioning benefits.</span></span>|
|<span data-ttu-id="4f843-140">warning</span><span class="sxs-lookup"><span data-stu-id="4f843-140">warning</span></span>                | <span data-ttu-id="4f843-141">Указывает, что право на использование, скорее всего, находится в льготной отсрочке из-за нарушения платежа.</span><span class="sxs-lookup"><span data-stu-id="4f843-141">Indicates that the usage right is in grace likely due to payment violation.</span></span> <span data-ttu-id="4f843-142">Это состояние можно использовать для напоминаия об ожидающих платежах или для ухудшения работы.</span><span class="sxs-lookup"><span data-stu-id="4f843-142">This state can be used to either remind of pending payment or offer a degraded experience.</span></span>|
|<span data-ttu-id="4f843-143">suspended</span><span class="sxs-lookup"><span data-stu-id="4f843-143">suspended</span></span>                | <span data-ttu-id="4f843-144">Указывает, что право на использование, скорее всего, приостановлено из-за нарушения платежа</span><span class="sxs-lookup"><span data-stu-id="4f843-144">Indicates that the usage right is suspended likely due to Payment violation</span></span>|
|<span data-ttu-id="4f843-145">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="4f843-145">unknownFutureValue</span></span>      | <span data-ttu-id="4f843-146">Значение Sentinel, чтобы указать будущие значения.</span><span class="sxs-lookup"><span data-stu-id="4f843-146">Sentinel value to indicate future values.</span></span> |

><span data-ttu-id="4f843-147">**Примечание.** Преимущество можно получить только в активных состояниях и состояниях предупреждений.</span><span class="sxs-lookup"><span data-stu-id="4f843-147">**Note:** Only the active and warning states represent a usable benefit.</span></span> <span data-ttu-id="4f843-148">Все остальные состояния следует рассматривать как не в результате чего полезное преимущество.</span><span class="sxs-lookup"><span data-stu-id="4f843-148">All other states should be treated as not resulting in a usable benefit.</span></span>



## <a name="relationships"></a><span data-ttu-id="4f843-149">Связи</span><span class="sxs-lookup"><span data-stu-id="4f843-149">Relationships</span></span>

<span data-ttu-id="4f843-150">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f843-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f843-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4f843-151">JSON representation</span></span>

<span data-ttu-id="4f843-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f843-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.usageRight",
  "id": "String (identifier)",
  "catalogId": "String",
  "serviceIdentifier": "String",
  "state": "String"
}
```

