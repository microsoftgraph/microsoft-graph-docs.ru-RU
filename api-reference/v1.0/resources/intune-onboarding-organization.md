---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2e4fffa10e81ba83a28fd6eebfc3ba4bf870d7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441744"
---
# <a name="organization-resource-type"></a><span data-ttu-id="d9476-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="d9476-103">organization resource type</span></span>

<span data-ttu-id="d9476-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9476-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9476-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9476-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9476-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="d9476-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="d9476-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d9476-107">Methods</span></span>
|<span data-ttu-id="d9476-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d9476-108">Method</span></span>|<span data-ttu-id="d9476-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d9476-109">Return Type</span></span>|<span data-ttu-id="d9476-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d9476-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9476-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="d9476-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="d9476-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="d9476-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="d9476-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="d9476-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="d9476-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="d9476-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="d9476-115">organization</span><span class="sxs-lookup"><span data-stu-id="d9476-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="d9476-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="d9476-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="d9476-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="d9476-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="d9476-118">organization</span><span class="sxs-lookup"><span data-stu-id="d9476-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="d9476-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="d9476-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="d9476-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="d9476-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="d9476-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d9476-121">Int32</span></span>|<span data-ttu-id="d9476-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="d9476-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="d9476-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9476-123">Properties</span></span>
|<span data-ttu-id="d9476-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9476-124">Property</span></span>|<span data-ttu-id="d9476-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d9476-125">Type</span></span>|<span data-ttu-id="d9476-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d9476-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9476-127">id</span><span class="sxs-lookup"><span data-stu-id="d9476-127">id</span></span>|<span data-ttu-id="d9476-128">String</span><span class="sxs-lookup"><span data-stu-id="d9476-128">String</span></span>|<span data-ttu-id="d9476-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="d9476-129">The GUID for the object.</span></span>|
|<span data-ttu-id="d9476-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="d9476-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="d9476-131">мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="d9476-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="d9476-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="d9476-132">Mobile device management authority.</span></span> <span data-ttu-id="d9476-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="d9476-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9476-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="d9476-134">Relationships</span></span>
<span data-ttu-id="d9476-135">Нет</span><span class="sxs-lookup"><span data-stu-id="d9476-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9476-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9476-136">JSON Representation</span></span>
<span data-ttu-id="d9476-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9476-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->







