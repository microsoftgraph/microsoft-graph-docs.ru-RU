---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76ef47ee4db5d7858ac476fd12db1615180bd18b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998018"
---
# <a name="organization-resource-type"></a><span data-ttu-id="248c6-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="248c6-103">organization resource type</span></span>

> <span data-ttu-id="248c6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="248c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="248c6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="248c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="248c6-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="248c6-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="248c6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="248c6-107">Methods</span></span>
|<span data-ttu-id="248c6-108">Метод</span><span class="sxs-lookup"><span data-stu-id="248c6-108">Method</span></span>|<span data-ttu-id="248c6-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="248c6-109">Return Type</span></span>|<span data-ttu-id="248c6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="248c6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="248c6-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="248c6-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="248c6-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="248c6-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="248c6-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="248c6-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="248c6-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="248c6-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="248c6-115">organization</span><span class="sxs-lookup"><span data-stu-id="248c6-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="248c6-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="248c6-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="248c6-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="248c6-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="248c6-118">organization</span><span class="sxs-lookup"><span data-stu-id="248c6-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="248c6-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="248c6-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="248c6-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="248c6-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="248c6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="248c6-121">Int32</span></span>|<span data-ttu-id="248c6-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="248c6-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="248c6-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="248c6-123">Properties</span></span>
|<span data-ttu-id="248c6-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="248c6-124">Property</span></span>|<span data-ttu-id="248c6-125">Тип</span><span class="sxs-lookup"><span data-stu-id="248c6-125">Type</span></span>|<span data-ttu-id="248c6-126">Описание</span><span class="sxs-lookup"><span data-stu-id="248c6-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="248c6-127">id</span><span class="sxs-lookup"><span data-stu-id="248c6-127">id</span></span>|<span data-ttu-id="248c6-128">String</span><span class="sxs-lookup"><span data-stu-id="248c6-128">String</span></span>|<span data-ttu-id="248c6-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="248c6-129">The GUID for the object.</span></span>|
|<span data-ttu-id="248c6-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="248c6-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="248c6-131">Мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="248c6-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="248c6-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="248c6-132">Mobile device management authority.</span></span> <span data-ttu-id="248c6-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="248c6-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="248c6-134">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="248c6-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="248c6-135">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="248c6-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="248c6-136">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="248c6-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="248c6-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="248c6-137">Relationships</span></span>
<span data-ttu-id="248c6-138">Нет</span><span class="sxs-lookup"><span data-stu-id="248c6-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="248c6-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="248c6-139">JSON Representation</span></span>
<span data-ttu-id="248c6-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="248c6-140">Here is a JSON representation of the resource.</span></span>
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





