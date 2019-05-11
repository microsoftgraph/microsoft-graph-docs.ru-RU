---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c871ba51733195947243fa9b22824156108f5eb7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949887"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="e5051-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="e5051-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="e5051-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5051-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5051-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5051-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5051-106">Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.</span><span class="sxs-lookup"><span data-stu-id="e5051-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="e5051-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e5051-107">Methods</span></span>
|<span data-ttu-id="e5051-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e5051-108">Method</span></span>|<span data-ttu-id="e5051-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e5051-109">Return Type</span></span>|<span data-ttu-id="e5051-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e5051-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5051-111">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="e5051-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="e5051-112">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e5051-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="e5051-113">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="e5051-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="e5051-114">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="e5051-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="e5051-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="e5051-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="e5051-116">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="e5051-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5051-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5051-117">Properties</span></span>
|<span data-ttu-id="e5051-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5051-118">Property</span></span>|<span data-ttu-id="e5051-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e5051-119">Type</span></span>|<span data-ttu-id="e5051-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e5051-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5051-121">id</span><span class="sxs-lookup"><span data-stu-id="e5051-121">id</span></span>|<span data-ttu-id="e5051-122">Строка</span><span class="sxs-lookup"><span data-stu-id="e5051-122">String</span></span>|<span data-ttu-id="e5051-123">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="e5051-123">The relationship entity id.</span></span>|
|<span data-ttu-id="e5051-124">targetId</span><span class="sxs-lookup"><span data-stu-id="e5051-124">targetId</span></span>|<span data-ttu-id="e5051-125">Строка</span><span class="sxs-lookup"><span data-stu-id="e5051-125">String</span></span>|<span data-ttu-id="e5051-126">Идентификатор приложения целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e5051-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="e5051-127">Таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="e5051-127">targetDisplayName</span></span>|<span data-ttu-id="e5051-128">Строка</span><span class="sxs-lookup"><span data-stu-id="e5051-128">String</span></span>|<span data-ttu-id="e5051-129">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e5051-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5051-130">Связи</span><span class="sxs-lookup"><span data-stu-id="e5051-130">Relationships</span></span>
<span data-ttu-id="e5051-131">Нет</span><span class="sxs-lookup"><span data-stu-id="e5051-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5051-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5051-132">JSON Representation</span></span>
<span data-ttu-id="e5051-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5051-133">Here is a JSON representation of the resource.</span></span>
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




