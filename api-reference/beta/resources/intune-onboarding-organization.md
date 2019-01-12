---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bc7a0fba8c5ecdc2b2a88062855e8b279721c45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990770"
---
# <a name="organization-resource-type"></a><span data-ttu-id="23139-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="23139-103">organization resource type</span></span>

> <span data-ttu-id="23139-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23139-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23139-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23139-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23139-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23139-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23139-107">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="23139-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="23139-108">Методы</span><span class="sxs-lookup"><span data-stu-id="23139-108">Methods</span></span>
|<span data-ttu-id="23139-109">Метод</span><span class="sxs-lookup"><span data-stu-id="23139-109">Method</span></span>|<span data-ttu-id="23139-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="23139-110">Return Type</span></span>|<span data-ttu-id="23139-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23139-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23139-112">Список организаций</span><span class="sxs-lookup"><span data-stu-id="23139-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="23139-113">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="23139-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="23139-114">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="23139-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="23139-115">Получение организации</span><span class="sxs-lookup"><span data-stu-id="23139-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="23139-116">organization</span><span class="sxs-lookup"><span data-stu-id="23139-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="23139-117">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="23139-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="23139-118">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="23139-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="23139-119">organization</span><span class="sxs-lookup"><span data-stu-id="23139-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="23139-120">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="23139-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="23139-121">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="23139-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="23139-122">Int32</span><span class="sxs-lookup"><span data-stu-id="23139-122">Int32</span></span>|<span data-ttu-id="23139-123">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="23139-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="23139-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="23139-124">Properties</span></span>
|<span data-ttu-id="23139-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="23139-125">Property</span></span>|<span data-ttu-id="23139-126">Тип</span><span class="sxs-lookup"><span data-stu-id="23139-126">Type</span></span>|<span data-ttu-id="23139-127">Описание</span><span class="sxs-lookup"><span data-stu-id="23139-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23139-128">id</span><span class="sxs-lookup"><span data-stu-id="23139-128">id</span></span>|<span data-ttu-id="23139-129">String</span><span class="sxs-lookup"><span data-stu-id="23139-129">String</span></span>|<span data-ttu-id="23139-130">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="23139-130">The GUID for the object.</span></span>|
|<span data-ttu-id="23139-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="23139-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="23139-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="23139-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="23139-133">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="23139-133">Mobile device management authority.</span></span> <span data-ttu-id="23139-134">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="23139-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="23139-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="23139-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="23139-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="23139-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="23139-137">Параметр соединителя сертификата.</span><span class="sxs-lookup"><span data-stu-id="23139-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23139-138">Связи</span><span class="sxs-lookup"><span data-stu-id="23139-138">Relationships</span></span>
<span data-ttu-id="23139-139">Нет</span><span class="sxs-lookup"><span data-stu-id="23139-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23139-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23139-140">JSON Representation</span></span>
<span data-ttu-id="23139-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23139-141">Here is a JSON representation of the resource.</span></span>
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





