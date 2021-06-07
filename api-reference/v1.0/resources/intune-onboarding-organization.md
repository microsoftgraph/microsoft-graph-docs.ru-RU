---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2af65c341f665fd358d03619a3cd3606723df123
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754953"
---
# <a name="organization-resource-type"></a><span data-ttu-id="2b617-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="2b617-103">organization resource type</span></span>

<span data-ttu-id="2b617-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b617-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b617-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b617-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b617-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="2b617-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="2b617-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2b617-107">Methods</span></span>
|<span data-ttu-id="2b617-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2b617-108">Method</span></span>|<span data-ttu-id="2b617-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2b617-109">Return Type</span></span>|<span data-ttu-id="2b617-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b617-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2b617-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="2b617-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="2b617-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="2b617-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="2b617-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="2b617-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="2b617-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="2b617-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="2b617-115">organization</span><span class="sxs-lookup"><span data-stu-id="2b617-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="2b617-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="2b617-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="2b617-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="2b617-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="2b617-118">organization</span><span class="sxs-lookup"><span data-stu-id="2b617-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="2b617-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="2b617-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="2b617-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="2b617-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="2b617-121">Int32</span><span class="sxs-lookup"><span data-stu-id="2b617-121">Int32</span></span>|<span data-ttu-id="2b617-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="2b617-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="2b617-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b617-123">Properties</span></span>
|<span data-ttu-id="2b617-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b617-124">Property</span></span>|<span data-ttu-id="2b617-125">Тип</span><span class="sxs-lookup"><span data-stu-id="2b617-125">Type</span></span>|<span data-ttu-id="2b617-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2b617-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b617-127">id</span><span class="sxs-lookup"><span data-stu-id="2b617-127">id</span></span>|<span data-ttu-id="2b617-128">String</span><span class="sxs-lookup"><span data-stu-id="2b617-128">String</span></span>|<span data-ttu-id="2b617-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="2b617-129">The GUID for the object.</span></span>|
|<span data-ttu-id="2b617-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="2b617-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="2b617-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="2b617-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="2b617-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="2b617-132">Mobile device management authority.</span></span> <span data-ttu-id="2b617-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="2b617-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b617-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="2b617-134">Relationships</span></span>
<span data-ttu-id="2b617-135">Нет</span><span class="sxs-lookup"><span data-stu-id="2b617-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b617-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b617-136">JSON Representation</span></span>
<span data-ttu-id="2b617-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b617-137">Here is a JSON representation of the resource.</span></span>
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




