---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af29752aaf54b5695d17dd78b1e93aab87755130
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375438"
---
# <a name="organization-resource-type"></a><span data-ttu-id="c4b18-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="c4b18-103">organization resource type</span></span>

> <span data-ttu-id="c4b18-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4b18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4b18-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4b18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4b18-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="c4b18-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="c4b18-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c4b18-107">Methods</span></span>
|<span data-ttu-id="c4b18-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c4b18-108">Method</span></span>|<span data-ttu-id="c4b18-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4b18-109">Return Type</span></span>|<span data-ttu-id="c4b18-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c4b18-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c4b18-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="c4b18-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="c4b18-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="c4b18-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="c4b18-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="c4b18-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="c4b18-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="c4b18-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="c4b18-115">organization</span><span class="sxs-lookup"><span data-stu-id="c4b18-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="c4b18-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="c4b18-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="c4b18-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="c4b18-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="c4b18-118">organization</span><span class="sxs-lookup"><span data-stu-id="c4b18-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="c4b18-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="c4b18-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="c4b18-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="c4b18-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="c4b18-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c4b18-121">Int32</span></span>|<span data-ttu-id="c4b18-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="c4b18-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="c4b18-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4b18-123">Properties</span></span>
|<span data-ttu-id="c4b18-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4b18-124">Property</span></span>|<span data-ttu-id="c4b18-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c4b18-125">Type</span></span>|<span data-ttu-id="c4b18-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c4b18-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4b18-127">id</span><span class="sxs-lookup"><span data-stu-id="c4b18-127">id</span></span>|<span data-ttu-id="c4b18-128">String</span><span class="sxs-lookup"><span data-stu-id="c4b18-128">String</span></span>|<span data-ttu-id="c4b18-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="c4b18-129">The GUID for the object.</span></span>|
|<span data-ttu-id="c4b18-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="c4b18-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="c4b18-131">мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="c4b18-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="c4b18-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="c4b18-132">Mobile device management authority.</span></span> <span data-ttu-id="c4b18-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="c4b18-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="c4b18-134">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="c4b18-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="c4b18-135">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="c4b18-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="c4b18-136">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="c4b18-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4b18-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="c4b18-137">Relationships</span></span>
<span data-ttu-id="c4b18-138">Нет</span><span class="sxs-lookup"><span data-stu-id="c4b18-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4b18-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4b18-139">JSON Representation</span></span>
<span data-ttu-id="c4b18-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4b18-140">Here is a JSON representation of the resource.</span></span>
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



