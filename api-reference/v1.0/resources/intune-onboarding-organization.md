---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
ms.openlocfilehash: ddc3b47777ea586a0f31c0d1d18aaa5727c828e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026471"
---
# <a name="organization-resource-type"></a><span data-ttu-id="bb30c-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="bb30c-103">organization resource type</span></span>

> <span data-ttu-id="bb30c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bb30c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb30c-105">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="bb30c-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="bb30c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bb30c-106">Methods</span></span>
|<span data-ttu-id="bb30c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bb30c-107">Method</span></span>|<span data-ttu-id="bb30c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb30c-108">Return Type</span></span>|<span data-ttu-id="bb30c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bb30c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb30c-110">Список организаций</span><span class="sxs-lookup"><span data-stu-id="bb30c-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="bb30c-111">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="bb30c-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="bb30c-112">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="bb30c-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="bb30c-113">Получение организации</span><span class="sxs-lookup"><span data-stu-id="bb30c-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="bb30c-114">organization</span><span class="sxs-lookup"><span data-stu-id="bb30c-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="bb30c-115">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="bb30c-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="bb30c-116">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="bb30c-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="bb30c-117">organization</span><span class="sxs-lookup"><span data-stu-id="bb30c-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="bb30c-118">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="bb30c-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="bb30c-119">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="bb30c-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="bb30c-120">Int32</span><span class="sxs-lookup"><span data-stu-id="bb30c-120">Int32</span></span>|<span data-ttu-id="bb30c-121">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="bb30c-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="bb30c-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb30c-122">Properties</span></span>
|<span data-ttu-id="bb30c-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb30c-123">Property</span></span>|<span data-ttu-id="bb30c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="bb30c-124">Type</span></span>|<span data-ttu-id="bb30c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bb30c-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb30c-126">id</span><span class="sxs-lookup"><span data-stu-id="bb30c-126">id</span></span>|<span data-ttu-id="bb30c-127">String</span><span class="sxs-lookup"><span data-stu-id="bb30c-127">String</span></span>|<span data-ttu-id="bb30c-128">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="bb30c-128">The GUID for the object.</span></span>|
|<span data-ttu-id="bb30c-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="bb30c-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="bb30c-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="bb30c-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="bb30c-131">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="bb30c-131">Mobile device management authority.</span></span> <span data-ttu-id="bb30c-132">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="bb30c-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb30c-133">Связи</span><span class="sxs-lookup"><span data-stu-id="bb30c-133">Relationships</span></span>
<span data-ttu-id="bb30c-134">Нет</span><span class="sxs-lookup"><span data-stu-id="bb30c-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb30c-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb30c-135">JSON Representation</span></span>
<span data-ttu-id="bb30c-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb30c-136">Here is a JSON representation of the resource.</span></span>
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

