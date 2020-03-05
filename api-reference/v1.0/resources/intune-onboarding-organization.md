---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c7f832fdce72f2490a45b3dae206eb7de28c686
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448027"
---
# <a name="organization-resource-type"></a><span data-ttu-id="305b4-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="305b4-103">organization resource type</span></span>

<span data-ttu-id="305b4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="305b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="305b4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="305b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="305b4-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="305b4-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="305b4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="305b4-107">Methods</span></span>
|<span data-ttu-id="305b4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="305b4-108">Method</span></span>|<span data-ttu-id="305b4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="305b4-109">Return Type</span></span>|<span data-ttu-id="305b4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="305b4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="305b4-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="305b4-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="305b4-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="305b4-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="305b4-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="305b4-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="305b4-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="305b4-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="305b4-115">organization</span><span class="sxs-lookup"><span data-stu-id="305b4-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="305b4-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="305b4-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="305b4-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="305b4-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="305b4-118">organization</span><span class="sxs-lookup"><span data-stu-id="305b4-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="305b4-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="305b4-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="305b4-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="305b4-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="305b4-121">Int32</span><span class="sxs-lookup"><span data-stu-id="305b4-121">Int32</span></span>|<span data-ttu-id="305b4-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="305b4-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="305b4-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="305b4-123">Properties</span></span>
|<span data-ttu-id="305b4-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="305b4-124">Property</span></span>|<span data-ttu-id="305b4-125">Тип</span><span class="sxs-lookup"><span data-stu-id="305b4-125">Type</span></span>|<span data-ttu-id="305b4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="305b4-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="305b4-127">id</span><span class="sxs-lookup"><span data-stu-id="305b4-127">id</span></span>|<span data-ttu-id="305b4-128">String</span><span class="sxs-lookup"><span data-stu-id="305b4-128">String</span></span>|<span data-ttu-id="305b4-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="305b4-129">The GUID for the object.</span></span>|
|<span data-ttu-id="305b4-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="305b4-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="305b4-131">мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="305b4-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="305b4-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="305b4-132">Mobile device management authority.</span></span> <span data-ttu-id="305b4-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="305b4-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="305b4-134">Связи</span><span class="sxs-lookup"><span data-stu-id="305b4-134">Relationships</span></span>
<span data-ttu-id="305b4-135">Нет</span><span class="sxs-lookup"><span data-stu-id="305b4-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="305b4-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="305b4-136">JSON Representation</span></span>
<span data-ttu-id="305b4-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="305b4-137">Here is a JSON representation of the resource.</span></span>
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




