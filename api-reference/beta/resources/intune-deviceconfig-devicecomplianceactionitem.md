---
title: Тип ресурса deviceComplianceActionItem
description: Конфигурация запланированного действия
author: tfitzmac
ms.openlocfilehash: d2df3b7eaf62c5a50e24f7b64a797b7bb91c2264
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308731"
---
# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="ee324-103">Тип ресурса deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-103">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="ee324-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee324-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee324-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee324-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee324-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ee324-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee324-107">Конфигурация запланированного действия</span><span class="sxs-lookup"><span data-stu-id="ee324-107">Scheduled Action Configuration</span></span>
## <a name="methods"></a><span data-ttu-id="ee324-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ee324-108">Methods</span></span>
|<span data-ttu-id="ee324-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ee324-109">Method</span></span>|<span data-ttu-id="ee324-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ee324-110">Return Type</span></span>|<span data-ttu-id="ee324-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ee324-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee324-112">Список объектов deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-112">List deviceComplianceActionItems</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|<span data-ttu-id="ee324-113">Коллекция [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)</span><span class="sxs-lookup"><span data-stu-id="ee324-113">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="ee324-114">Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="ee324-114">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="ee324-115">Получение объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-115">Get deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[<span data-ttu-id="ee324-116">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-116">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="ee324-117">Чтение свойств и связей объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="ee324-117">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="ee324-118">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-118">Create deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[<span data-ttu-id="ee324-119">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-119">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="ee324-120">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="ee324-120">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="ee324-121">Удаление объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-121">Delete deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|<span data-ttu-id="ee324-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ee324-122">None</span></span>|<span data-ttu-id="ee324-123">Удаляет объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="ee324-123">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="ee324-124">Обновление объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-124">Update deviceComplianceActionItem</span></span>](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[<span data-ttu-id="ee324-125">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ee324-125">deviceComplianceActionItem</span></span>](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|<span data-ttu-id="ee324-126">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="ee324-126">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee324-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee324-127">Properties</span></span>
|<span data-ttu-id="ee324-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee324-128">Property</span></span>|<span data-ttu-id="ee324-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ee324-129">Type</span></span>|<span data-ttu-id="ee324-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ee324-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee324-131">id</span><span class="sxs-lookup"><span data-stu-id="ee324-131">id</span></span>|<span data-ttu-id="ee324-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ee324-132">String</span></span>|<span data-ttu-id="ee324-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee324-133">Key of the entity.</span></span>|
|<span data-ttu-id="ee324-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="ee324-134">gracePeriodHours</span></span>|<span data-ttu-id="ee324-135">Int32</span><span class="sxs-lookup"><span data-stu-id="ee324-135">Int32</span></span>|<span data-ttu-id="ee324-136">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="ee324-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="ee324-137">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="ee324-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="ee324-138">actionType</span><span class="sxs-lookup"><span data-stu-id="ee324-138">actionType</span></span>|[<span data-ttu-id="ee324-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="ee324-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="ee324-140">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="ee324-140">What action to take.</span></span> <span data-ttu-id="ee324-141">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="ee324-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="ee324-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="ee324-142">notificationTemplateId</span></span>|<span data-ttu-id="ee324-143">String</span><span class="sxs-lookup"><span data-stu-id="ee324-143">String</span></span>|<span data-ttu-id="ee324-144">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="ee324-144">What notification Message template to use</span></span>|
|<span data-ttu-id="ee324-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="ee324-145">notificationMessageCCList</span></span>|<span data-ttu-id="ee324-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ee324-146">String collection</span></span>|<span data-ttu-id="ee324-147">Список идентификаторов групп, которым будет отправлена копия этого сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="ee324-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee324-148">Связи</span><span class="sxs-lookup"><span data-stu-id="ee324-148">Relationships</span></span>
<span data-ttu-id="ee324-149">Нет</span><span class="sxs-lookup"><span data-stu-id="ee324-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ee324-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee324-150">JSON Representation</span></span>
<span data-ttu-id="ee324-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee324-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```





