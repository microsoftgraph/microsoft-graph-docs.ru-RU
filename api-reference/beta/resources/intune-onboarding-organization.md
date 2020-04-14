---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5f4fcca12b08b49533c583d38e089d0c3b5335c4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371426"
---
# <a name="organization-resource-type"></a><span data-ttu-id="50dc4-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="50dc4-103">organization resource type</span></span>

<span data-ttu-id="50dc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50dc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50dc4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50dc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50dc4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50dc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50dc4-107">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="50dc4-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="50dc4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="50dc4-108">Methods</span></span>
|<span data-ttu-id="50dc4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="50dc4-109">Method</span></span>|<span data-ttu-id="50dc4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="50dc4-110">Return Type</span></span>|<span data-ttu-id="50dc4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="50dc4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50dc4-112">Список организаций</span><span class="sxs-lookup"><span data-stu-id="50dc4-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="50dc4-113">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="50dc4-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="50dc4-114">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="50dc4-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="50dc4-115">Get organization</span><span class="sxs-lookup"><span data-stu-id="50dc4-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="50dc4-116">organization</span><span class="sxs-lookup"><span data-stu-id="50dc4-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="50dc4-117">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="50dc4-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="50dc4-118">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="50dc4-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="50dc4-119">organization</span><span class="sxs-lookup"><span data-stu-id="50dc4-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="50dc4-120">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="50dc4-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="50dc4-121">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="50dc4-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="50dc4-122">Int32</span><span class="sxs-lookup"><span data-stu-id="50dc4-122">Int32</span></span>|<span data-ttu-id="50dc4-123">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="50dc4-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="50dc4-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="50dc4-124">Properties</span></span>
|<span data-ttu-id="50dc4-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="50dc4-125">Property</span></span>|<span data-ttu-id="50dc4-126">Тип</span><span class="sxs-lookup"><span data-stu-id="50dc4-126">Type</span></span>|<span data-ttu-id="50dc4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="50dc4-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50dc4-128">id</span><span class="sxs-lookup"><span data-stu-id="50dc4-128">id</span></span>|<span data-ttu-id="50dc4-129">String</span><span class="sxs-lookup"><span data-stu-id="50dc4-129">String</span></span>|<span data-ttu-id="50dc4-130">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="50dc4-130">The GUID for the object.</span></span>|
|<span data-ttu-id="50dc4-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="50dc4-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="50dc4-132">мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="50dc4-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="50dc4-133">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="50dc4-133">Mobile device management authority.</span></span> <span data-ttu-id="50dc4-134">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="50dc4-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="50dc4-135">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="50dc4-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="50dc4-136">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="50dc4-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="50dc4-137">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="50dc4-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50dc4-138">Связи</span><span class="sxs-lookup"><span data-stu-id="50dc4-138">Relationships</span></span>
<span data-ttu-id="50dc4-139">Нет</span><span class="sxs-lookup"><span data-stu-id="50dc4-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50dc4-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50dc4-140">JSON Representation</span></span>
<span data-ttu-id="50dc4-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50dc4-141">Here is a JSON representation of the resource.</span></span>
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
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```



