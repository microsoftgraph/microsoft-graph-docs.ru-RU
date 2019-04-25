---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9806c1d263710ecaef2c04af89926e7568ad94da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566418"
---
# <a name="organization-resource-type"></a><span data-ttu-id="e41d8-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="e41d8-103">organization resource type</span></span>

> <span data-ttu-id="e41d8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e41d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e41d8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e41d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e41d8-106">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="e41d8-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="e41d8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e41d8-107">Methods</span></span>
|<span data-ttu-id="e41d8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e41d8-108">Method</span></span>|<span data-ttu-id="e41d8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e41d8-109">Return Type</span></span>|<span data-ttu-id="e41d8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e41d8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e41d8-111">Список организаций</span><span class="sxs-lookup"><span data-stu-id="e41d8-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="e41d8-112">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="e41d8-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="e41d8-113">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e41d8-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="e41d8-114">Get organization</span><span class="sxs-lookup"><span data-stu-id="e41d8-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="e41d8-115">organization</span><span class="sxs-lookup"><span data-stu-id="e41d8-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e41d8-116">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e41d8-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e41d8-117">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="e41d8-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="e41d8-118">organization</span><span class="sxs-lookup"><span data-stu-id="e41d8-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e41d8-119">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e41d8-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e41d8-120">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e41d8-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="e41d8-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e41d8-121">Int32</span></span>|<span data-ttu-id="e41d8-122">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="e41d8-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="e41d8-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="e41d8-123">Properties</span></span>
|<span data-ttu-id="e41d8-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="e41d8-124">Property</span></span>|<span data-ttu-id="e41d8-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e41d8-125">Type</span></span>|<span data-ttu-id="e41d8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e41d8-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e41d8-127">id</span><span class="sxs-lookup"><span data-stu-id="e41d8-127">id</span></span>|<span data-ttu-id="e41d8-128">String</span><span class="sxs-lookup"><span data-stu-id="e41d8-128">String</span></span>|<span data-ttu-id="e41d8-129">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="e41d8-129">The GUID for the object.</span></span>|
|<span data-ttu-id="e41d8-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e41d8-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e41d8-131">Мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="e41d8-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="e41d8-132">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="e41d8-132">Mobile device management authority.</span></span> <span data-ttu-id="e41d8-133">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="e41d8-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="e41d8-134">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="e41d8-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="e41d8-135">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="e41d8-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="e41d8-136">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e41d8-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e41d8-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="e41d8-137">Relationships</span></span>
<span data-ttu-id="e41d8-138">Нет</span><span class="sxs-lookup"><span data-stu-id="e41d8-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e41d8-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e41d8-139">JSON Representation</span></span>
<span data-ttu-id="e41d8-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e41d8-140">Here is a JSON representation of the resource.</span></span>
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





