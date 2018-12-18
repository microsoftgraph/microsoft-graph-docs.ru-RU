---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: tfitzmac
ms.openlocfilehash: da2d127dc5ba44187d8a3a066f5fe261d3dee859
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322850"
---
# <a name="organization-resource-type"></a><span data-ttu-id="3411a-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="3411a-103">organization resource type</span></span>

> <span data-ttu-id="3411a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3411a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3411a-105">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="3411a-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="3411a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3411a-106">Methods</span></span>
|<span data-ttu-id="3411a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3411a-107">Method</span></span>|<span data-ttu-id="3411a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3411a-108">Return Type</span></span>|<span data-ttu-id="3411a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3411a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3411a-110">Список организаций</span><span class="sxs-lookup"><span data-stu-id="3411a-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="3411a-111">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="3411a-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="3411a-112">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="3411a-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="3411a-113">Получение организации</span><span class="sxs-lookup"><span data-stu-id="3411a-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="3411a-114">organization</span><span class="sxs-lookup"><span data-stu-id="3411a-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="3411a-115">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="3411a-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="3411a-116">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="3411a-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="3411a-117">organization</span><span class="sxs-lookup"><span data-stu-id="3411a-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="3411a-118">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="3411a-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="3411a-119">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="3411a-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="3411a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="3411a-120">Int32</span></span>|<span data-ttu-id="3411a-121">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="3411a-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="3411a-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="3411a-122">Properties</span></span>
|<span data-ttu-id="3411a-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="3411a-123">Property</span></span>|<span data-ttu-id="3411a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3411a-124">Type</span></span>|<span data-ttu-id="3411a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3411a-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3411a-126">id</span><span class="sxs-lookup"><span data-stu-id="3411a-126">id</span></span>|<span data-ttu-id="3411a-127">Строка</span><span class="sxs-lookup"><span data-stu-id="3411a-127">String</span></span>|<span data-ttu-id="3411a-128">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="3411a-128">The GUID for the object.</span></span>|
|<span data-ttu-id="3411a-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="3411a-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="3411a-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="3411a-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="3411a-131">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="3411a-131">Mobile device management authority.</span></span> <span data-ttu-id="3411a-132">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="3411a-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3411a-133">Связи</span><span class="sxs-lookup"><span data-stu-id="3411a-133">Relationships</span></span>
<span data-ttu-id="3411a-134">Нет</span><span class="sxs-lookup"><span data-stu-id="3411a-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3411a-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3411a-135">JSON Representation</span></span>
<span data-ttu-id="3411a-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3411a-136">Here is a JSON representation of the resource.</span></span>
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

