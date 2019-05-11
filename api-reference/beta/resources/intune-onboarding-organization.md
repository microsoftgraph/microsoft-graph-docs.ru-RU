---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c587d5a15fa0161e10058eec4a2f8c6183a28a1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940157"
---
# <a name="organization-resource-type"></a><span data-ttu-id="87a09-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="87a09-103">organization resource type</span></span>

> <span data-ttu-id="87a09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87a09-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87a09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87a09-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="87a09-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="87a09-107">Методы</span><span class="sxs-lookup"><span data-stu-id="87a09-107">Methods</span></span>
|<span data-ttu-id="87a09-108">Метод</span><span class="sxs-lookup"><span data-stu-id="87a09-108">Method</span></span>|<span data-ttu-id="87a09-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="87a09-109">Return Type</span></span>|<span data-ttu-id="87a09-110">Описание</span><span class="sxs-lookup"><span data-stu-id="87a09-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87a09-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="87a09-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="87a09-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="87a09-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="87a09-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="87a09-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="87a09-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="87a09-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="87a09-115">organization</span><span class="sxs-lookup"><span data-stu-id="87a09-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="87a09-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="87a09-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="87a09-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="87a09-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="87a09-118">organization</span><span class="sxs-lookup"><span data-stu-id="87a09-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="87a09-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="87a09-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="87a09-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="87a09-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="87a09-121">Int32</span><span class="sxs-lookup"><span data-stu-id="87a09-121">Int32</span></span>|<span data-ttu-id="87a09-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="87a09-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="87a09-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="87a09-123">Properties</span></span>
|<span data-ttu-id="87a09-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="87a09-124">Property</span></span>|<span data-ttu-id="87a09-125">Тип</span><span class="sxs-lookup"><span data-stu-id="87a09-125">Type</span></span>|<span data-ttu-id="87a09-126">Описание</span><span class="sxs-lookup"><span data-stu-id="87a09-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87a09-127">id</span><span class="sxs-lookup"><span data-stu-id="87a09-127">id</span></span>|<span data-ttu-id="87a09-128">Строка</span><span class="sxs-lookup"><span data-stu-id="87a09-128">String</span></span>|<span data-ttu-id="87a09-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="87a09-129">The GUID for the object.</span></span>|
|<span data-ttu-id="87a09-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="87a09-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="87a09-131">Мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="87a09-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="87a09-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="87a09-132">Mobile device management authority.</span></span> <span data-ttu-id="87a09-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="87a09-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="87a09-134">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="87a09-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="87a09-135">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="87a09-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="87a09-136">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="87a09-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87a09-137">Связи</span><span class="sxs-lookup"><span data-stu-id="87a09-137">Relationships</span></span>
<span data-ttu-id="87a09-138">Нет</span><span class="sxs-lookup"><span data-stu-id="87a09-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87a09-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87a09-139">JSON Representation</span></span>
<span data-ttu-id="87a09-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87a09-140">Here is a JSON representation of the resource.</span></span>
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




