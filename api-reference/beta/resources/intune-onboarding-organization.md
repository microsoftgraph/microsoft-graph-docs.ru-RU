---
title: Тип ресурса organization
description: Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7c6f99c378bc7fd53f473419a5ca4f4350f7c57b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812049"
---
# <a name="organization-resource-type"></a><span data-ttu-id="6e33b-103">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="6e33b-103">organization resource type</span></span>

> <span data-ttu-id="6e33b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e33b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e33b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e33b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e33b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6e33b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e33b-107">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="6e33b-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="6e33b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6e33b-108">Methods</span></span>
|<span data-ttu-id="6e33b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6e33b-109">Method</span></span>|<span data-ttu-id="6e33b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6e33b-110">Return Type</span></span>|<span data-ttu-id="6e33b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6e33b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e33b-112">Список организаций</span><span class="sxs-lookup"><span data-stu-id="6e33b-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="6e33b-113">Коллекция объектов [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="6e33b-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="6e33b-114">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="6e33b-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="6e33b-115">Получение организации</span><span class="sxs-lookup"><span data-stu-id="6e33b-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="6e33b-116">organization</span><span class="sxs-lookup"><span data-stu-id="6e33b-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="6e33b-117">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="6e33b-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="6e33b-118">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="6e33b-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="6e33b-119">organization</span><span class="sxs-lookup"><span data-stu-id="6e33b-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="6e33b-120">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="6e33b-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="6e33b-121">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="6e33b-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="6e33b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="6e33b-122">Int32</span></span>|<span data-ttu-id="6e33b-123">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="6e33b-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="6e33b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e33b-124">Properties</span></span>
|<span data-ttu-id="6e33b-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e33b-125">Property</span></span>|<span data-ttu-id="6e33b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="6e33b-126">Type</span></span>|<span data-ttu-id="6e33b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6e33b-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e33b-128">id</span><span class="sxs-lookup"><span data-stu-id="6e33b-128">id</span></span>|<span data-ttu-id="6e33b-129">Строка</span><span class="sxs-lookup"><span data-stu-id="6e33b-129">String</span></span>|<span data-ttu-id="6e33b-130">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="6e33b-130">The GUID for the object.</span></span>|
|<span data-ttu-id="6e33b-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="6e33b-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="6e33b-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="6e33b-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="6e33b-133">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="6e33b-133">Mobile device management authority.</span></span> <span data-ttu-id="6e33b-134">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="6e33b-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="6e33b-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="6e33b-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="6e33b-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="6e33b-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="6e33b-137">Параметр соединителя сертификата.</span><span class="sxs-lookup"><span data-stu-id="6e33b-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e33b-138">Связи</span><span class="sxs-lookup"><span data-stu-id="6e33b-138">Relationships</span></span>
<span data-ttu-id="6e33b-139">Нет</span><span class="sxs-lookup"><span data-stu-id="6e33b-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6e33b-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e33b-140">JSON Representation</span></span>
<span data-ttu-id="6e33b-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e33b-141">Here is a JSON representation of the resource.</span></span>
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





