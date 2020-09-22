---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает отношение между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2c7af932983b9b3657a94a7448149b75b3c8eea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076350"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="c4244-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="c4244-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="c4244-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4244-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4244-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4244-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4244-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4244-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4244-107">Описывает отношение между двумя мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="c4244-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="c4244-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c4244-108">Methods</span></span>
|<span data-ttu-id="c4244-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c4244-109">Method</span></span>|<span data-ttu-id="c4244-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4244-110">Return Type</span></span>|<span data-ttu-id="c4244-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c4244-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c4244-112">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="c4244-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="c4244-113">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c4244-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="c4244-114">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="c4244-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="c4244-115">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="c4244-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="c4244-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="c4244-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="c4244-117">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="c4244-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4244-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4244-118">Properties</span></span>
|<span data-ttu-id="c4244-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4244-119">Property</span></span>|<span data-ttu-id="c4244-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c4244-120">Type</span></span>|<span data-ttu-id="c4244-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c4244-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4244-122">id</span><span class="sxs-lookup"><span data-stu-id="c4244-122">id</span></span>|<span data-ttu-id="c4244-123">String</span><span class="sxs-lookup"><span data-stu-id="c4244-123">String</span></span>|<span data-ttu-id="c4244-124">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="c4244-124">The relationship entity id.</span></span>|
|<span data-ttu-id="c4244-125">targetId</span><span class="sxs-lookup"><span data-stu-id="c4244-125">targetId</span></span>|<span data-ttu-id="c4244-126">String</span><span class="sxs-lookup"><span data-stu-id="c4244-126">String</span></span>|<span data-ttu-id="c4244-127">Идентификатор приложения целевого приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="c4244-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="c4244-128">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="c4244-128">targetDisplayName</span></span>|<span data-ttu-id="c4244-129">String</span><span class="sxs-lookup"><span data-stu-id="c4244-129">String</span></span>|<span data-ttu-id="c4244-130">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c4244-130">The target mobile app's display name.</span></span>|
|<span data-ttu-id="c4244-131">targetType</span><span class="sxs-lookup"><span data-stu-id="c4244-131">targetType</span></span>|[<span data-ttu-id="c4244-132">мобилеаппрелатионшиптипе</span><span class="sxs-lookup"><span data-stu-id="c4244-132">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="c4244-133">Тип связи, указывающий, является ли целевой объект родительским или дочерним.</span><span class="sxs-lookup"><span data-stu-id="c4244-133">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="c4244-134">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="c4244-134">Possible values are: `child`, `parent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4244-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="c4244-135">Relationships</span></span>
<span data-ttu-id="c4244-136">Нет</span><span class="sxs-lookup"><span data-stu-id="c4244-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4244-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4244-137">JSON Representation</span></span>
<span data-ttu-id="c4244-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4244-138">Here is a JSON representation of the resource.</span></span>
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






