---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e1afa1ded131844f687fa2dbad1a8e07639b264
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524626"
---
# <a name="organization-resource-type"></a><span data-ttu-id="85334-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="85334-103">organization resource type</span></span>

> <span data-ttu-id="85334-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85334-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85334-105">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="85334-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="85334-106">Методы</span><span class="sxs-lookup"><span data-stu-id="85334-106">Methods</span></span>
|<span data-ttu-id="85334-107">Метод</span><span class="sxs-lookup"><span data-stu-id="85334-107">Method</span></span>|<span data-ttu-id="85334-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85334-108">Return Type</span></span>|<span data-ttu-id="85334-109">Описание</span><span class="sxs-lookup"><span data-stu-id="85334-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="85334-110">Список организаций</span><span class="sxs-lookup"><span data-stu-id="85334-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="85334-111">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="85334-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="85334-112">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="85334-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="85334-113">Get organization</span><span class="sxs-lookup"><span data-stu-id="85334-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="85334-114">organization</span><span class="sxs-lookup"><span data-stu-id="85334-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="85334-115">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="85334-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="85334-116">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="85334-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="85334-117">organization</span><span class="sxs-lookup"><span data-stu-id="85334-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="85334-118">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="85334-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="85334-119">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="85334-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="85334-120">Int32</span><span class="sxs-lookup"><span data-stu-id="85334-120">Int32</span></span>|<span data-ttu-id="85334-121">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="85334-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="85334-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="85334-122">Properties</span></span>
|<span data-ttu-id="85334-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="85334-123">Property</span></span>|<span data-ttu-id="85334-124">Тип</span><span class="sxs-lookup"><span data-stu-id="85334-124">Type</span></span>|<span data-ttu-id="85334-125">Описание</span><span class="sxs-lookup"><span data-stu-id="85334-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85334-126">id</span><span class="sxs-lookup"><span data-stu-id="85334-126">id</span></span>|<span data-ttu-id="85334-127">String</span><span class="sxs-lookup"><span data-stu-id="85334-127">String</span></span>|<span data-ttu-id="85334-128">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="85334-128">The GUID for the object.</span></span>|
|<span data-ttu-id="85334-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="85334-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="85334-130">Мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="85334-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="85334-131">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="85334-131">Mobile device management authority.</span></span> <span data-ttu-id="85334-132">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="85334-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85334-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="85334-133">Relationships</span></span>
<span data-ttu-id="85334-134">Нет</span><span class="sxs-lookup"><span data-stu-id="85334-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85334-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85334-135">JSON Representation</span></span>
<span data-ttu-id="85334-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85334-136">Here is a JSON representation of the resource.</span></span>
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



