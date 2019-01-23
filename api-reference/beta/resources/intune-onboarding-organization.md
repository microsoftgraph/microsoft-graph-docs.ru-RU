---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b47ec69063998a935640f05d04a17bfc5714c8d8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398235"
---
# <a name="organization-resource-type"></a><span data-ttu-id="ed644-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="ed644-103">organization resource type</span></span>

> <span data-ttu-id="ed644-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed644-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ed644-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed644-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed644-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed644-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed644-107">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="ed644-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="ed644-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ed644-108">Methods</span></span>
|<span data-ttu-id="ed644-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ed644-109">Method</span></span>|<span data-ttu-id="ed644-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed644-110">Return Type</span></span>|<span data-ttu-id="ed644-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed644-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed644-112">Список организаций</span><span class="sxs-lookup"><span data-stu-id="ed644-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="ed644-113">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="ed644-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="ed644-114">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ed644-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="ed644-115">Получение организации</span><span class="sxs-lookup"><span data-stu-id="ed644-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="ed644-116">organization</span><span class="sxs-lookup"><span data-stu-id="ed644-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ed644-117">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ed644-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ed644-118">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="ed644-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="ed644-119">organization</span><span class="sxs-lookup"><span data-stu-id="ed644-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ed644-120">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ed644-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ed644-121">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ed644-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="ed644-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ed644-122">Int32</span></span>|<span data-ttu-id="ed644-123">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="ed644-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="ed644-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed644-124">Properties</span></span>
|<span data-ttu-id="ed644-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed644-125">Property</span></span>|<span data-ttu-id="ed644-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ed644-126">Type</span></span>|<span data-ttu-id="ed644-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ed644-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed644-128">id</span><span class="sxs-lookup"><span data-stu-id="ed644-128">id</span></span>|<span data-ttu-id="ed644-129">String</span><span class="sxs-lookup"><span data-stu-id="ed644-129">String</span></span>|<span data-ttu-id="ed644-130">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="ed644-130">The GUID for the object.</span></span>|
|<span data-ttu-id="ed644-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ed644-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="ed644-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="ed644-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="ed644-133">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="ed644-133">Mobile device management authority.</span></span> <span data-ttu-id="ed644-134">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="ed644-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="ed644-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="ed644-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="ed644-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="ed644-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="ed644-137">Параметр соединителя сертификата.</span><span class="sxs-lookup"><span data-stu-id="ed644-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed644-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="ed644-138">Relationships</span></span>
<span data-ttu-id="ed644-139">Нет</span><span class="sxs-lookup"><span data-stu-id="ed644-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed644-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed644-140">JSON Representation</span></span>
<span data-ttu-id="ed644-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed644-141">Here is a JSON representation of the resource.</span></span>
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




