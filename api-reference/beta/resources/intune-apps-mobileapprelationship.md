---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e193878122a3a43cd97d05ad1bdc5bea302fcc8a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991823"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="7924f-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="7924f-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="7924f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7924f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7924f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7924f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7924f-106">Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.</span><span class="sxs-lookup"><span data-stu-id="7924f-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="7924f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7924f-107">Methods</span></span>
|<span data-ttu-id="7924f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7924f-108">Method</span></span>|<span data-ttu-id="7924f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7924f-109">Return Type</span></span>|<span data-ttu-id="7924f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7924f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7924f-111">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="7924f-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="7924f-112">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="7924f-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="7924f-113">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="7924f-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="7924f-114">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="7924f-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="7924f-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="7924f-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="7924f-116">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="7924f-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7924f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="7924f-117">Properties</span></span>
|<span data-ttu-id="7924f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="7924f-118">Property</span></span>|<span data-ttu-id="7924f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7924f-119">Type</span></span>|<span data-ttu-id="7924f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7924f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7924f-121">id</span><span class="sxs-lookup"><span data-stu-id="7924f-121">id</span></span>|<span data-ttu-id="7924f-122">String</span><span class="sxs-lookup"><span data-stu-id="7924f-122">String</span></span>|<span data-ttu-id="7924f-123">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="7924f-123">The relationship entity id.</span></span>|
|<span data-ttu-id="7924f-124">targetId</span><span class="sxs-lookup"><span data-stu-id="7924f-124">targetId</span></span>|<span data-ttu-id="7924f-125">String</span><span class="sxs-lookup"><span data-stu-id="7924f-125">String</span></span>|<span data-ttu-id="7924f-126">Идентификатор приложения целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7924f-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="7924f-127">Таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="7924f-127">targetDisplayName</span></span>|<span data-ttu-id="7924f-128">String</span><span class="sxs-lookup"><span data-stu-id="7924f-128">String</span></span>|<span data-ttu-id="7924f-129">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7924f-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7924f-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="7924f-130">Relationships</span></span>
<span data-ttu-id="7924f-131">Нет</span><span class="sxs-lookup"><span data-stu-id="7924f-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7924f-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7924f-132">JSON Representation</span></span>
<span data-ttu-id="7924f-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7924f-133">Here is a JSON representation of the resource.</span></span>
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





