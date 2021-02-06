---
title: Тип ресурса usageRight
description: Содержит сведения об usageRight, назначенного пользователем или устройством
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d3d7ad0de7eb6929e54b7d3d692c6e562e9da76d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130413"
---
# <a name="usageright-resource-type"></a><span data-ttu-id="22a93-103">Тип ресурса usageRight</span><span class="sxs-lookup"><span data-stu-id="22a93-103">usageRight resource type</span></span>

<span data-ttu-id="22a93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22a93-105">Право на использование представляет лицензию, которая есть у пользователя или устройства для сторонних программ, основанных на приложениях питания, или для подписок на устройства (только для устройств).</span><span class="sxs-lookup"><span data-stu-id="22a93-105">A usage right represents a license that a user or device has for either third party software built on power apps or for device based subscriptions (device only).</span></span>

## <a name="methods"></a><span data-ttu-id="22a93-106">Методы</span><span class="sxs-lookup"><span data-stu-id="22a93-106">Methods</span></span>

|<span data-ttu-id="22a93-107">Метод</span><span class="sxs-lookup"><span data-stu-id="22a93-107">Method</span></span>|<span data-ttu-id="22a93-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="22a93-108">Return type</span></span>|<span data-ttu-id="22a93-109">Описание</span><span class="sxs-lookup"><span data-stu-id="22a93-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22a93-110">Список user usageRights</span><span class="sxs-lookup"><span data-stu-id="22a93-110">List user usageRights</span></span>](../api/user-list-usagerights.md)|<span data-ttu-id="22a93-111">Коллекция [usageRight](../resources/usageright.md)</span><span class="sxs-lookup"><span data-stu-id="22a93-111">[usageRight](../resources/usageright.md) collection</span></span>|<span data-ttu-id="22a93-112">Получите список прав на использование для пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a93-112">Get the list of usage rights for a user.</span></span>|
|[<span data-ttu-id="22a93-113">Список устройств usageRights</span><span class="sxs-lookup"><span data-stu-id="22a93-113">List device usageRights</span></span>](../api/device-list-usagerights.md)|<span data-ttu-id="22a93-114">Коллекция [usageRight](../resources/usageright.md)</span><span class="sxs-lookup"><span data-stu-id="22a93-114">[usageRight](../resources/usageright.md) collection</span></span>|<span data-ttu-id="22a93-115">Получите список прав на использование для устройства.</span><span class="sxs-lookup"><span data-stu-id="22a93-115">Get the list of usage rights for a device.</span></span>|

## <a name="properties"></a><span data-ttu-id="22a93-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="22a93-116">Properties</span></span>

|<span data-ttu-id="22a93-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="22a93-117">Property</span></span>|<span data-ttu-id="22a93-118">Тип</span><span class="sxs-lookup"><span data-stu-id="22a93-118">Type</span></span>|<span data-ttu-id="22a93-119">Описание</span><span class="sxs-lookup"><span data-stu-id="22a93-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a93-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="22a93-120">catalogId</span></span>|<span data-ttu-id="22a93-121">Строка</span><span class="sxs-lookup"><span data-stu-id="22a93-121">String</span></span>|<span data-ttu-id="22a93-122">ИД продукта, соответствующий правом на использование.</span><span class="sxs-lookup"><span data-stu-id="22a93-122">Product id corresponding to the usage right.</span></span>|
|<span data-ttu-id="22a93-123">id</span><span class="sxs-lookup"><span data-stu-id="22a93-123">id</span></span>|<span data-ttu-id="22a93-124">Строка</span><span class="sxs-lookup"><span data-stu-id="22a93-124">String</span></span>|<span data-ttu-id="22a93-125">ИД права на использование.</span><span class="sxs-lookup"><span data-stu-id="22a93-125">The id of the usage right.</span></span>|
|<span data-ttu-id="22a93-126">serviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="22a93-126">serviceIdentifier</span></span>|<span data-ttu-id="22a93-127">Строка</span><span class="sxs-lookup"><span data-stu-id="22a93-127">String</span></span>|<span data-ttu-id="22a93-128">Идентификатор службы, соответствующей правом на использование.</span><span class="sxs-lookup"><span data-stu-id="22a93-128">Identifier of the service corresponding to the usage right.</span></span>|
|<span data-ttu-id="22a93-129">state</span><span class="sxs-lookup"><span data-stu-id="22a93-129">state</span></span>|<span data-ttu-id="22a93-130">usageRightState</span><span class="sxs-lookup"><span data-stu-id="22a93-130">usageRightState</span></span>|<span data-ttu-id="22a93-131">Состояние права на использование.</span><span class="sxs-lookup"><span data-stu-id="22a93-131">The state of the usage right.</span></span> <span data-ttu-id="22a93-132">Возможные значения: `active`, `inactive`, `warning`, `suspended`.</span><span class="sxs-lookup"><span data-stu-id="22a93-132">Possible values are: `active`, `inactive`, `warning`, `suspended`.</span></span>|

### <a name="usagerightstate-values"></a><span data-ttu-id="22a93-133">значения usageRightState</span><span class="sxs-lookup"><span data-stu-id="22a93-133">usageRightState values</span></span> 

| <span data-ttu-id="22a93-134">Member</span><span class="sxs-lookup"><span data-stu-id="22a93-134">Member</span></span>             |  <span data-ttu-id="22a93-135">Описание</span><span class="sxs-lookup"><span data-stu-id="22a93-135">Description</span></span>               |
| :----------------- |  :------------------------ |
|<span data-ttu-id="22a93-136">active</span><span class="sxs-lookup"><span data-stu-id="22a93-136">active</span></span>              | <span data-ttu-id="22a93-137">Указывает, что право на использование активно и может использоваться для предоставления преимуществ.</span><span class="sxs-lookup"><span data-stu-id="22a93-137">Indicates that the usage right is active and can be used for provisioning benefits.</span></span>|
|<span data-ttu-id="22a93-138">неактивный</span><span class="sxs-lookup"><span data-stu-id="22a93-138">inactive</span></span>                | <span data-ttu-id="22a93-139">Указывает, что право на использование не является активным и не может использоваться для предоставления преимуществ.</span><span class="sxs-lookup"><span data-stu-id="22a93-139">Indicates that the usage right is not active and cannot be used for provisioning benefits.</span></span>|
|<span data-ttu-id="22a93-140">warning</span><span class="sxs-lookup"><span data-stu-id="22a93-140">warning</span></span>                | <span data-ttu-id="22a93-141">Указывает, что право на использование, скорее всего, находится в льготной отсрочке из-за нарушения платежа.</span><span class="sxs-lookup"><span data-stu-id="22a93-141">Indicates that the usage right is in grace likely due to payment violation.</span></span> <span data-ttu-id="22a93-142">Это состояние можно использовать для напоминаия об ожидающих платежах или для ухудшения работы.</span><span class="sxs-lookup"><span data-stu-id="22a93-142">This state can be used to either remind of pending payment or offer a degraded experience.</span></span>|
|<span data-ttu-id="22a93-143">suspended</span><span class="sxs-lookup"><span data-stu-id="22a93-143">suspended</span></span>                | <span data-ttu-id="22a93-144">Указывает, что право на использование, скорее всего, приостановлено из-за нарушения платежа</span><span class="sxs-lookup"><span data-stu-id="22a93-144">Indicates that the usage right is suspended likely due to Payment violation</span></span>|
|<span data-ttu-id="22a93-145">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="22a93-145">unknownFutureValue</span></span>      | <span data-ttu-id="22a93-146">Значение Sentinel, чтобы указать будущие значения.</span><span class="sxs-lookup"><span data-stu-id="22a93-146">Sentinel value to indicate future values.</span></span> |

><span data-ttu-id="22a93-147">**Примечание.** Преимущества, которые можно получить, представляют только активные состояния и состояния предупреждений.</span><span class="sxs-lookup"><span data-stu-id="22a93-147">**Note:** Only the active and warning states represent a usable benefit.</span></span> <span data-ttu-id="22a93-148">Все остальные состояния должны рассматриваться как не приумещающие преимущества.</span><span class="sxs-lookup"><span data-stu-id="22a93-148">All other states should be treated as not resulting in a usable benefit.</span></span>



## <a name="relationships"></a><span data-ttu-id="22a93-149">Связи</span><span class="sxs-lookup"><span data-stu-id="22a93-149">Relationships</span></span>

<span data-ttu-id="22a93-150">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="22a93-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="22a93-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="22a93-151">JSON representation</span></span>

<span data-ttu-id="22a93-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22a93-152">The following is a JSON representation of the resource.</span></span>
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

