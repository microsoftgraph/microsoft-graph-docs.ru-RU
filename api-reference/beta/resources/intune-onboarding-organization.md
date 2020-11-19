---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30dbbb5b7a86b39acceabc2ebf8df74caafca9c9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259545"
---
# <a name="organization-resource-type"></a><span data-ttu-id="412af-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="412af-103">organization resource type</span></span>

<span data-ttu-id="412af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="412af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="412af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="412af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="412af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="412af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="412af-107">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="412af-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="412af-108">Методы</span><span class="sxs-lookup"><span data-stu-id="412af-108">Methods</span></span>
|<span data-ttu-id="412af-109">Метод</span><span class="sxs-lookup"><span data-stu-id="412af-109">Method</span></span>|<span data-ttu-id="412af-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="412af-110">Return Type</span></span>|<span data-ttu-id="412af-111">Описание</span><span class="sxs-lookup"><span data-stu-id="412af-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="412af-112">Список организаций</span><span class="sxs-lookup"><span data-stu-id="412af-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="412af-113">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="412af-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="412af-114">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="412af-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="412af-115">Get organization</span><span class="sxs-lookup"><span data-stu-id="412af-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="412af-116">organization</span><span class="sxs-lookup"><span data-stu-id="412af-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="412af-117">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="412af-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="412af-118">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="412af-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="412af-119">organization</span><span class="sxs-lookup"><span data-stu-id="412af-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="412af-120">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="412af-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="412af-121">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="412af-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="412af-122">Int32</span><span class="sxs-lookup"><span data-stu-id="412af-122">Int32</span></span>|<span data-ttu-id="412af-123">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="412af-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="412af-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="412af-124">Properties</span></span>
|<span data-ttu-id="412af-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="412af-125">Property</span></span>|<span data-ttu-id="412af-126">Тип</span><span class="sxs-lookup"><span data-stu-id="412af-126">Type</span></span>|<span data-ttu-id="412af-127">Описание</span><span class="sxs-lookup"><span data-stu-id="412af-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="412af-128">id</span><span class="sxs-lookup"><span data-stu-id="412af-128">id</span></span>|<span data-ttu-id="412af-129">String</span><span class="sxs-lookup"><span data-stu-id="412af-129">String</span></span>|<span data-ttu-id="412af-130">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="412af-130">The GUID for the object.</span></span>|
|<span data-ttu-id="412af-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="412af-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="412af-132">мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="412af-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="412af-133">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="412af-133">Mobile device management authority.</span></span> <span data-ttu-id="412af-134">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="412af-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="412af-135">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="412af-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="412af-136">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="412af-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="412af-137">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="412af-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="412af-138">Связи</span><span class="sxs-lookup"><span data-stu-id="412af-138">Relationships</span></span>
<span data-ttu-id="412af-139">Нет</span><span class="sxs-lookup"><span data-stu-id="412af-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="412af-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="412af-140">JSON Representation</span></span>
<span data-ttu-id="412af-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="412af-141">Here is a JSON representation of the resource.</span></span>
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




