---
title: Тип ресурса Мобилеаппрелатионшип
description: Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3841ab8e10bb1306dcd2f7b5b3002ded0bd2fcbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491430"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="55ea3-103">Тип ресурса Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="55ea3-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="55ea3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="55ea3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55ea3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ea3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55ea3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55ea3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55ea3-107">Описывает связь для дочернего мобильного приложения с родительским мобильным приложением.</span><span class="sxs-lookup"><span data-stu-id="55ea3-107">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="55ea3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="55ea3-108">Methods</span></span>
|<span data-ttu-id="55ea3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="55ea3-109">Method</span></span>|<span data-ttu-id="55ea3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55ea3-110">Return Type</span></span>|<span data-ttu-id="55ea3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55ea3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55ea3-112">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="55ea3-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="55ea3-113">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="55ea3-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="55ea3-114">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="55ea3-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="55ea3-115">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="55ea3-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="55ea3-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="55ea3-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="55ea3-117">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="55ea3-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="55ea3-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="55ea3-118">Properties</span></span>
|<span data-ttu-id="55ea3-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="55ea3-119">Property</span></span>|<span data-ttu-id="55ea3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="55ea3-120">Type</span></span>|<span data-ttu-id="55ea3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="55ea3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55ea3-122">id</span><span class="sxs-lookup"><span data-stu-id="55ea3-122">id</span></span>|<span data-ttu-id="55ea3-123">String</span><span class="sxs-lookup"><span data-stu-id="55ea3-123">String</span></span>|<span data-ttu-id="55ea3-124">Идентификатор сущности отношения.</span><span class="sxs-lookup"><span data-stu-id="55ea3-124">The relationship entity id.</span></span>|
|<span data-ttu-id="55ea3-125">targetId</span><span class="sxs-lookup"><span data-stu-id="55ea3-125">targetId</span></span>|<span data-ttu-id="55ea3-126">String</span><span class="sxs-lookup"><span data-stu-id="55ea3-126">String</span></span>|<span data-ttu-id="55ea3-127">Идентификатор приложения целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="55ea3-127">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="55ea3-128">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="55ea3-128">targetDisplayName</span></span>|<span data-ttu-id="55ea3-129">String</span><span class="sxs-lookup"><span data-stu-id="55ea3-129">String</span></span>|<span data-ttu-id="55ea3-130">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="55ea3-130">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55ea3-131">Связи</span><span class="sxs-lookup"><span data-stu-id="55ea3-131">Relationships</span></span>
<span data-ttu-id="55ea3-132">Нет</span><span class="sxs-lookup"><span data-stu-id="55ea3-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55ea3-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55ea3-133">JSON Representation</span></span>
<span data-ttu-id="55ea3-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55ea3-134">Here is a JSON representation of the resource.</span></span>
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



