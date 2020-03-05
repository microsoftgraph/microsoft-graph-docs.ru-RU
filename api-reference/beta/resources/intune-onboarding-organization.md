---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a24fb6529d65a4cac3b9674933148205856d33c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527710"
---
# <a name="organization-resource-type"></a><span data-ttu-id="05a83-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="05a83-103">organization resource type</span></span>

<span data-ttu-id="05a83-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="05a83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05a83-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05a83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05a83-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05a83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05a83-107">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="05a83-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="05a83-108">Методы</span><span class="sxs-lookup"><span data-stu-id="05a83-108">Methods</span></span>
|<span data-ttu-id="05a83-109">Метод</span><span class="sxs-lookup"><span data-stu-id="05a83-109">Method</span></span>|<span data-ttu-id="05a83-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05a83-110">Return Type</span></span>|<span data-ttu-id="05a83-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05a83-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05a83-112">Список организаций</span><span class="sxs-lookup"><span data-stu-id="05a83-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="05a83-113">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="05a83-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="05a83-114">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="05a83-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="05a83-115">Get organization</span><span class="sxs-lookup"><span data-stu-id="05a83-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="05a83-116">organization</span><span class="sxs-lookup"><span data-stu-id="05a83-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="05a83-117">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="05a83-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="05a83-118">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="05a83-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="05a83-119">organization</span><span class="sxs-lookup"><span data-stu-id="05a83-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="05a83-120">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="05a83-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="05a83-121">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="05a83-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="05a83-122">Int32</span><span class="sxs-lookup"><span data-stu-id="05a83-122">Int32</span></span>|<span data-ttu-id="05a83-123">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="05a83-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="05a83-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="05a83-124">Properties</span></span>
|<span data-ttu-id="05a83-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="05a83-125">Property</span></span>|<span data-ttu-id="05a83-126">Тип</span><span class="sxs-lookup"><span data-stu-id="05a83-126">Type</span></span>|<span data-ttu-id="05a83-127">Описание</span><span class="sxs-lookup"><span data-stu-id="05a83-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05a83-128">id</span><span class="sxs-lookup"><span data-stu-id="05a83-128">id</span></span>|<span data-ttu-id="05a83-129">String</span><span class="sxs-lookup"><span data-stu-id="05a83-129">String</span></span>|<span data-ttu-id="05a83-130">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="05a83-130">The GUID for the object.</span></span>|
|<span data-ttu-id="05a83-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="05a83-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="05a83-132">мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="05a83-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="05a83-133">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="05a83-133">Mobile device management authority.</span></span> <span data-ttu-id="05a83-134">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="05a83-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="05a83-135">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="05a83-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="05a83-136">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="05a83-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="05a83-137">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="05a83-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05a83-138">Связи</span><span class="sxs-lookup"><span data-stu-id="05a83-138">Relationships</span></span>
<span data-ttu-id="05a83-139">Нет</span><span class="sxs-lookup"><span data-stu-id="05a83-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05a83-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05a83-140">JSON Representation</span></span>
<span data-ttu-id="05a83-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05a83-141">Here is a JSON representation of the resource.</span></span>
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



