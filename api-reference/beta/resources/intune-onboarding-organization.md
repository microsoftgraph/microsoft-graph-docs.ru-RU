---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46186451d55247c3a405df83955113cfcf05e143
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958629"
---
# <a name="organization-resource-type"></a><span data-ttu-id="7ff5c-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="7ff5c-103">organization resource type</span></span>

> <span data-ttu-id="7ff5c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ff5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ff5c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ff5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ff5c-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="7ff5c-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="7ff5c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7ff5c-107">Methods</span></span>
|<span data-ttu-id="7ff5c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7ff5c-108">Method</span></span>|<span data-ttu-id="7ff5c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ff5c-109">Return Type</span></span>|<span data-ttu-id="7ff5c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff5c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ff5c-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="7ff5c-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="7ff5c-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="7ff5c-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="7ff5c-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="7ff5c-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="7ff5c-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="7ff5c-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="7ff5c-115">organization</span><span class="sxs-lookup"><span data-stu-id="7ff5c-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="7ff5c-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="7ff5c-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="7ff5c-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="7ff5c-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="7ff5c-118">organization</span><span class="sxs-lookup"><span data-stu-id="7ff5c-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="7ff5c-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="7ff5c-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="7ff5c-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="7ff5c-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="7ff5c-121">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff5c-121">Int32</span></span>|<span data-ttu-id="7ff5c-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="7ff5c-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="7ff5c-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ff5c-123">Properties</span></span>
|<span data-ttu-id="7ff5c-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ff5c-124">Property</span></span>|<span data-ttu-id="7ff5c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff5c-125">Type</span></span>|<span data-ttu-id="7ff5c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff5c-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff5c-127">id</span><span class="sxs-lookup"><span data-stu-id="7ff5c-127">id</span></span>|<span data-ttu-id="7ff5c-128">String</span><span class="sxs-lookup"><span data-stu-id="7ff5c-128">String</span></span>|<span data-ttu-id="7ff5c-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="7ff5c-129">The GUID for the object.</span></span>|
|<span data-ttu-id="7ff5c-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="7ff5c-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="7ff5c-131">Мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="7ff5c-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="7ff5c-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="7ff5c-132">Mobile device management authority.</span></span> <span data-ttu-id="7ff5c-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="7ff5c-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="7ff5c-134">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="7ff5c-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="7ff5c-135">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="7ff5c-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="7ff5c-136">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="7ff5c-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ff5c-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="7ff5c-137">Relationships</span></span>
<span data-ttu-id="7ff5c-138">Нет</span><span class="sxs-lookup"><span data-stu-id="7ff5c-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ff5c-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ff5c-139">JSON Representation</span></span>
<span data-ttu-id="7ff5c-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ff5c-140">Here is a JSON representation of the resource.</span></span>
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





