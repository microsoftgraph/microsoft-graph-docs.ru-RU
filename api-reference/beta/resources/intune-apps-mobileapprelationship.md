---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает отношение между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c6143147e84112fe4c83c620cddca3cfe1547bf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48719731"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="60e25-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="60e25-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="60e25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60e25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60e25-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60e25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60e25-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60e25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60e25-107">Описывает отношение между двумя мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="60e25-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="60e25-108">Методы</span><span class="sxs-lookup"><span data-stu-id="60e25-108">Methods</span></span>
|<span data-ttu-id="60e25-109">Метод</span><span class="sxs-lookup"><span data-stu-id="60e25-109">Method</span></span>|<span data-ttu-id="60e25-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60e25-110">Return Type</span></span>|<span data-ttu-id="60e25-111">Описание</span><span class="sxs-lookup"><span data-stu-id="60e25-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60e25-112">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="60e25-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="60e25-113">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="60e25-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="60e25-114">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="60e25-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="60e25-115">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="60e25-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="60e25-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="60e25-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="60e25-117">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="60e25-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="60e25-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="60e25-118">Properties</span></span>
|<span data-ttu-id="60e25-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="60e25-119">Property</span></span>|<span data-ttu-id="60e25-120">Тип</span><span class="sxs-lookup"><span data-stu-id="60e25-120">Type</span></span>|<span data-ttu-id="60e25-121">Описание</span><span class="sxs-lookup"><span data-stu-id="60e25-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60e25-122">id</span><span class="sxs-lookup"><span data-stu-id="60e25-122">id</span></span>|<span data-ttu-id="60e25-123">Строка</span><span class="sxs-lookup"><span data-stu-id="60e25-123">String</span></span>|<span data-ttu-id="60e25-124">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="60e25-124">The relationship entity id.</span></span>|
|<span data-ttu-id="60e25-125">targetId</span><span class="sxs-lookup"><span data-stu-id="60e25-125">targetId</span></span>|<span data-ttu-id="60e25-126">Строка</span><span class="sxs-lookup"><span data-stu-id="60e25-126">String</span></span>|<span data-ttu-id="60e25-127">Идентификатор приложения целевого приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="60e25-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="60e25-128">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="60e25-128">targetDisplayName</span></span>|<span data-ttu-id="60e25-129">Строка</span><span class="sxs-lookup"><span data-stu-id="60e25-129">String</span></span>|<span data-ttu-id="60e25-130">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="60e25-130">The target mobile app's display name.</span></span>|
|<span data-ttu-id="60e25-131">targetType</span><span class="sxs-lookup"><span data-stu-id="60e25-131">targetType</span></span>|[<span data-ttu-id="60e25-132">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="60e25-132">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="60e25-133">Тип связи, указывающий, является ли целевой объект родительским или дочерним.</span><span class="sxs-lookup"><span data-stu-id="60e25-133">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="60e25-134">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="60e25-134">Possible values are: `child`, `parent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60e25-135">Связи</span><span class="sxs-lookup"><span data-stu-id="60e25-135">Relationships</span></span>
<span data-ttu-id="60e25-136">Нет</span><span class="sxs-lookup"><span data-stu-id="60e25-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60e25-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60e25-137">JSON Representation</span></span>
<span data-ttu-id="60e25-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60e25-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetType": "String"
}
```





