---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ed999914958578bfa4c39b99b27ff159827e207
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809302"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="32ee3-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="32ee3-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="32ee3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32ee3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32ee3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32ee3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32ee3-106">Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.</span><span class="sxs-lookup"><span data-stu-id="32ee3-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="32ee3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="32ee3-107">Methods</span></span>
|<span data-ttu-id="32ee3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="32ee3-108">Method</span></span>|<span data-ttu-id="32ee3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="32ee3-109">Return Type</span></span>|<span data-ttu-id="32ee3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="32ee3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="32ee3-111">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="32ee3-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="32ee3-112">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="32ee3-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="32ee3-113">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="32ee3-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="32ee3-114">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="32ee3-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="32ee3-115">Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="32ee3-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="32ee3-116">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="32ee3-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="32ee3-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="32ee3-117">Properties</span></span>
|<span data-ttu-id="32ee3-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="32ee3-118">Property</span></span>|<span data-ttu-id="32ee3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="32ee3-119">Type</span></span>|<span data-ttu-id="32ee3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="32ee3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32ee3-121">id</span><span class="sxs-lookup"><span data-stu-id="32ee3-121">id</span></span>|<span data-ttu-id="32ee3-122">String</span><span class="sxs-lookup"><span data-stu-id="32ee3-122">String</span></span>|<span data-ttu-id="32ee3-123">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="32ee3-123">The relationship entity id.</span></span>|
|<span data-ttu-id="32ee3-124">targetId</span><span class="sxs-lookup"><span data-stu-id="32ee3-124">targetId</span></span>|<span data-ttu-id="32ee3-125">String</span><span class="sxs-lookup"><span data-stu-id="32ee3-125">String</span></span>|<span data-ttu-id="32ee3-126">Идентификатор приложения целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="32ee3-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="32ee3-127">Таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="32ee3-127">targetDisplayName</span></span>|<span data-ttu-id="32ee3-128">String</span><span class="sxs-lookup"><span data-stu-id="32ee3-128">String</span></span>|<span data-ttu-id="32ee3-129">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="32ee3-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32ee3-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="32ee3-130">Relationships</span></span>
<span data-ttu-id="32ee3-131">Нет</span><span class="sxs-lookup"><span data-stu-id="32ee3-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32ee3-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32ee3-132">JSON Representation</span></span>
<span data-ttu-id="32ee3-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32ee3-133">Here is a JSON representation of the resource.</span></span>
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





