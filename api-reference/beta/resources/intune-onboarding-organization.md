---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd8481ddea83194c7e1b769c70518c9ddff3f894
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42778017"
---
# <a name="organization-resource-type"></a><span data-ttu-id="ee83d-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="ee83d-103">organization resource type</span></span>

> <span data-ttu-id="ee83d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee83d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee83d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee83d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee83d-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="ee83d-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="ee83d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ee83d-107">Methods</span></span>
|<span data-ttu-id="ee83d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ee83d-108">Method</span></span>|<span data-ttu-id="ee83d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ee83d-109">Return Type</span></span>|<span data-ttu-id="ee83d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ee83d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee83d-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="ee83d-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="ee83d-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="ee83d-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="ee83d-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ee83d-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="ee83d-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="ee83d-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="ee83d-115">organization</span><span class="sxs-lookup"><span data-stu-id="ee83d-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ee83d-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ee83d-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ee83d-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="ee83d-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="ee83d-118">organization</span><span class="sxs-lookup"><span data-stu-id="ee83d-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ee83d-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ee83d-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ee83d-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ee83d-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="ee83d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ee83d-121">Int32</span></span>|<span data-ttu-id="ee83d-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="ee83d-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="ee83d-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee83d-123">Properties</span></span>
|<span data-ttu-id="ee83d-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee83d-124">Property</span></span>|<span data-ttu-id="ee83d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ee83d-125">Type</span></span>|<span data-ttu-id="ee83d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ee83d-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee83d-127">id</span><span class="sxs-lookup"><span data-stu-id="ee83d-127">id</span></span>|<span data-ttu-id="ee83d-128">String</span><span class="sxs-lookup"><span data-stu-id="ee83d-128">String</span></span>|<span data-ttu-id="ee83d-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="ee83d-129">The GUID for the object.</span></span>|
|<span data-ttu-id="ee83d-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ee83d-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="ee83d-131">мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="ee83d-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="ee83d-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="ee83d-132">Mobile device management authority.</span></span> <span data-ttu-id="ee83d-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="ee83d-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="ee83d-134">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="ee83d-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="ee83d-135">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="ee83d-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="ee83d-136">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ee83d-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee83d-137">Связи</span><span class="sxs-lookup"><span data-stu-id="ee83d-137">Relationships</span></span>
<span data-ttu-id="ee83d-138">Нет</span><span class="sxs-lookup"><span data-stu-id="ee83d-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee83d-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee83d-139">JSON Representation</span></span>
<span data-ttu-id="ee83d-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee83d-140">Here is a JSON representation of the resource.</span></span>
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



