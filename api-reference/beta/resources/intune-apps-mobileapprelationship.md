---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80cf0fd5897d0ff3d1b3b3adc5343ad4c059442e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462584"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="949b5-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="949b5-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="949b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="949b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="949b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="949b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="949b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="949b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="949b5-107">Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.</span><span class="sxs-lookup"><span data-stu-id="949b5-107">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="949b5-108">Методы</span><span class="sxs-lookup"><span data-stu-id="949b5-108">Methods</span></span>
|<span data-ttu-id="949b5-109">Метод</span><span class="sxs-lookup"><span data-stu-id="949b5-109">Method</span></span>|<span data-ttu-id="949b5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="949b5-110">Return Type</span></span>|<span data-ttu-id="949b5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="949b5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="949b5-112">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="949b5-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="949b5-113">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="949b5-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="949b5-114">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="949b5-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="949b5-115">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="949b5-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="949b5-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="949b5-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="949b5-117">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="949b5-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="949b5-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="949b5-118">Properties</span></span>
|<span data-ttu-id="949b5-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="949b5-119">Property</span></span>|<span data-ttu-id="949b5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="949b5-120">Type</span></span>|<span data-ttu-id="949b5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="949b5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="949b5-122">id</span><span class="sxs-lookup"><span data-stu-id="949b5-122">id</span></span>|<span data-ttu-id="949b5-123">String</span><span class="sxs-lookup"><span data-stu-id="949b5-123">String</span></span>|<span data-ttu-id="949b5-124">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="949b5-124">The relationship entity id.</span></span>|
|<span data-ttu-id="949b5-125">targetId</span><span class="sxs-lookup"><span data-stu-id="949b5-125">targetId</span></span>|<span data-ttu-id="949b5-126">String</span><span class="sxs-lookup"><span data-stu-id="949b5-126">String</span></span>|<span data-ttu-id="949b5-127">Идентификатор приложения целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="949b5-127">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="949b5-128">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="949b5-128">targetDisplayName</span></span>|<span data-ttu-id="949b5-129">String</span><span class="sxs-lookup"><span data-stu-id="949b5-129">String</span></span>|<span data-ttu-id="949b5-130">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="949b5-130">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="949b5-131">Связи</span><span class="sxs-lookup"><span data-stu-id="949b5-131">Relationships</span></span>
<span data-ttu-id="949b5-132">Нет</span><span class="sxs-lookup"><span data-stu-id="949b5-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="949b5-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="949b5-133">JSON Representation</span></span>
<span data-ttu-id="949b5-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="949b5-134">Here is a JSON representation of the resource.</span></span>
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



