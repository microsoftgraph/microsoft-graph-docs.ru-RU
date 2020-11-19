---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает отношение между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22af70876075aa12b5493cfa413c79bd2c71c7cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217195"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="55c80-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="55c80-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="55c80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55c80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55c80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55c80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55c80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55c80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55c80-107">Описывает отношение между двумя мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="55c80-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="55c80-108">Методы</span><span class="sxs-lookup"><span data-stu-id="55c80-108">Methods</span></span>
|<span data-ttu-id="55c80-109">Метод</span><span class="sxs-lookup"><span data-stu-id="55c80-109">Method</span></span>|<span data-ttu-id="55c80-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55c80-110">Return Type</span></span>|<span data-ttu-id="55c80-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55c80-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55c80-112">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="55c80-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="55c80-113">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="55c80-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="55c80-114">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="55c80-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="55c80-115">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="55c80-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="55c80-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="55c80-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="55c80-117">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="55c80-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="55c80-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="55c80-118">Properties</span></span>
|<span data-ttu-id="55c80-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="55c80-119">Property</span></span>|<span data-ttu-id="55c80-120">Тип</span><span class="sxs-lookup"><span data-stu-id="55c80-120">Type</span></span>|<span data-ttu-id="55c80-121">Описание</span><span class="sxs-lookup"><span data-stu-id="55c80-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55c80-122">id</span><span class="sxs-lookup"><span data-stu-id="55c80-122">id</span></span>|<span data-ttu-id="55c80-123">String</span><span class="sxs-lookup"><span data-stu-id="55c80-123">String</span></span>|<span data-ttu-id="55c80-124">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="55c80-124">The relationship entity id.</span></span>|
|<span data-ttu-id="55c80-125">targetId</span><span class="sxs-lookup"><span data-stu-id="55c80-125">targetId</span></span>|<span data-ttu-id="55c80-126">String</span><span class="sxs-lookup"><span data-stu-id="55c80-126">String</span></span>|<span data-ttu-id="55c80-127">Идентификатор приложения целевого приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="55c80-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="55c80-128">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="55c80-128">targetDisplayName</span></span>|<span data-ttu-id="55c80-129">String</span><span class="sxs-lookup"><span data-stu-id="55c80-129">String</span></span>|<span data-ttu-id="55c80-130">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="55c80-130">The target mobile app's display name.</span></span>|
|<span data-ttu-id="55c80-131">таржетдисплайверсион</span><span class="sxs-lookup"><span data-stu-id="55c80-131">targetDisplayVersion</span></span>|<span data-ttu-id="55c80-132">String</span><span class="sxs-lookup"><span data-stu-id="55c80-132">String</span></span>|<span data-ttu-id="55c80-133">Версия отображения целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="55c80-133">The target mobile app's display version.</span></span>|
|<span data-ttu-id="55c80-134">таржетпублишер</span><span class="sxs-lookup"><span data-stu-id="55c80-134">targetPublisher</span></span>|<span data-ttu-id="55c80-135">String</span><span class="sxs-lookup"><span data-stu-id="55c80-135">String</span></span>|<span data-ttu-id="55c80-136">Издатель целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="55c80-136">The target mobile app's publisher.</span></span>|
|<span data-ttu-id="55c80-137">targetType</span><span class="sxs-lookup"><span data-stu-id="55c80-137">targetType</span></span>|[<span data-ttu-id="55c80-138">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="55c80-138">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="55c80-139">Тип связи, указывающий, является ли целевой объект родительским или дочерним.</span><span class="sxs-lookup"><span data-stu-id="55c80-139">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="55c80-140">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="55c80-140">Possible values are: `child`, `parent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55c80-141">Связи</span><span class="sxs-lookup"><span data-stu-id="55c80-141">Relationships</span></span>
<span data-ttu-id="55c80-142">Нет</span><span class="sxs-lookup"><span data-stu-id="55c80-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55c80-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55c80-143">JSON Representation</span></span>
<span data-ttu-id="55c80-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55c80-144">Here is a JSON representation of the resource.</span></span>
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
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String"
}
```




