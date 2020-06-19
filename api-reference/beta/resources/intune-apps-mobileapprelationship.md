---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает отношение между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d09d9d7604699ee89b6dccc0f2f980cef26225e7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790868"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="66e7d-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="66e7d-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="66e7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66e7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66e7d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66e7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66e7d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66e7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66e7d-107">Описывает отношение между двумя мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="66e7d-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="66e7d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="66e7d-108">Methods</span></span>
|<span data-ttu-id="66e7d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="66e7d-109">Method</span></span>|<span data-ttu-id="66e7d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="66e7d-110">Return Type</span></span>|<span data-ttu-id="66e7d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66e7d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66e7d-112">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="66e7d-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="66e7d-113">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="66e7d-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="66e7d-114">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="66e7d-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="66e7d-115">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="66e7d-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="66e7d-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="66e7d-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="66e7d-117">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="66e7d-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="66e7d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="66e7d-118">Properties</span></span>
|<span data-ttu-id="66e7d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="66e7d-119">Property</span></span>|<span data-ttu-id="66e7d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="66e7d-120">Type</span></span>|<span data-ttu-id="66e7d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="66e7d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66e7d-122">id</span><span class="sxs-lookup"><span data-stu-id="66e7d-122">id</span></span>|<span data-ttu-id="66e7d-123">String</span><span class="sxs-lookup"><span data-stu-id="66e7d-123">String</span></span>|<span data-ttu-id="66e7d-124">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="66e7d-124">The relationship entity id.</span></span>|
|<span data-ttu-id="66e7d-125">targetId</span><span class="sxs-lookup"><span data-stu-id="66e7d-125">targetId</span></span>|<span data-ttu-id="66e7d-126">String</span><span class="sxs-lookup"><span data-stu-id="66e7d-126">String</span></span>|<span data-ttu-id="66e7d-127">Идентификатор приложения целевого приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="66e7d-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="66e7d-128">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="66e7d-128">targetDisplayName</span></span>|<span data-ttu-id="66e7d-129">String</span><span class="sxs-lookup"><span data-stu-id="66e7d-129">String</span></span>|<span data-ttu-id="66e7d-130">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="66e7d-130">The target mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66e7d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="66e7d-131">Relationships</span></span>
<span data-ttu-id="66e7d-132">Нет</span><span class="sxs-lookup"><span data-stu-id="66e7d-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66e7d-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66e7d-133">JSON Representation</span></span>
<span data-ttu-id="66e7d-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66e7d-134">Here is a JSON representation of the resource.</span></span>
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
  "targetDisplayName": "String"
}
```



