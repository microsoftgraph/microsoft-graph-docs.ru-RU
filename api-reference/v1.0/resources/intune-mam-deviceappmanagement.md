---
title: Тип ресурса deviceAppManagement
description: Единичный объект управления приложениями на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8906e96a0218360bbe78d1c08dd4d8767568775
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752053"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="60aab-103">Тип ресурса deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="60aab-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="60aab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60aab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60aab-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60aab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60aab-106">Единичный объект управления приложениями на устройствах.</span><span class="sxs-lookup"><span data-stu-id="60aab-106">Device app management singleton entity.</span></span>

## <a name="methods"></a><span data-ttu-id="60aab-107">Методы</span><span class="sxs-lookup"><span data-stu-id="60aab-107">Methods</span></span>
|<span data-ttu-id="60aab-108">Метод</span><span class="sxs-lookup"><span data-stu-id="60aab-108">Method</span></span>|<span data-ttu-id="60aab-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60aab-109">Return Type</span></span>|<span data-ttu-id="60aab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="60aab-110">Description</span></span>|
|:---|:---|:---|

## <a name="properties"></a><span data-ttu-id="60aab-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="60aab-111">Properties</span></span>
|<span data-ttu-id="60aab-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="60aab-112">Property</span></span>|<span data-ttu-id="60aab-113">Тип</span><span class="sxs-lookup"><span data-stu-id="60aab-113">Type</span></span>|<span data-ttu-id="60aab-114">Описание</span><span class="sxs-lookup"><span data-stu-id="60aab-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60aab-115">id</span><span class="sxs-lookup"><span data-stu-id="60aab-115">id</span></span>|<span data-ttu-id="60aab-116">String</span><span class="sxs-lookup"><span data-stu-id="60aab-116">String</span></span>|<span data-ttu-id="60aab-117">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="60aab-117">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60aab-118">Связи</span><span class="sxs-lookup"><span data-stu-id="60aab-118">Relationships</span></span>
|<span data-ttu-id="60aab-119">Связь</span><span class="sxs-lookup"><span data-stu-id="60aab-119">Relationship</span></span>|<span data-ttu-id="60aab-120">Тип</span><span class="sxs-lookup"><span data-stu-id="60aab-120">Type</span></span>|<span data-ttu-id="60aab-121">Описание</span><span class="sxs-lookup"><span data-stu-id="60aab-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60aab-122">managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="60aab-122">managedAppPolicies</span></span>|<span data-ttu-id="60aab-123">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-123">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="60aab-124">Политики управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="60aab-124">Managed app policies.</span></span>|
|<span data-ttu-id="60aab-125">iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="60aab-125">iosManagedAppProtections</span></span>|<span data-ttu-id="60aab-126">Коллекция [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-126">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) collection</span></span>|<span data-ttu-id="60aab-127">Политики управляемых приложений для iOS.</span><span class="sxs-lookup"><span data-stu-id="60aab-127">iOS managed app policies.</span></span>|
|<span data-ttu-id="60aab-128">androidManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="60aab-128">androidManagedAppProtections</span></span>|<span data-ttu-id="60aab-129">Коллекция [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-129">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) collection</span></span>|<span data-ttu-id="60aab-130">Политики управляемых приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="60aab-130">Android managed app policies.</span></span>|
|<span data-ttu-id="60aab-131">defaultManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="60aab-131">defaultManagedAppProtections</span></span>|<span data-ttu-id="60aab-132">Коллекция [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-132">[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) collection</span></span>|<span data-ttu-id="60aab-133">Политики управляемых приложений по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="60aab-133">Default managed app policies.</span></span>|
|<span data-ttu-id="60aab-134">targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="60aab-134">targetedManagedAppConfigurations</span></span>|<span data-ttu-id="60aab-135">Коллекция [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-135">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="60aab-136">Целевые конфигурации управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="60aab-136">Targeted managed app configurations.</span></span>|
|<span data-ttu-id="60aab-137">mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="60aab-137">mdmWindowsInformationProtectionPolicies</span></span>|<span data-ttu-id="60aab-138">Коллекция [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-138">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="60aab-139">Windows Information Protection для приложений на устройствах, зарегистрированных с использованием MDM.</span><span class="sxs-lookup"><span data-stu-id="60aab-139">Windows information protection for apps running on devices which are MDM enrolled.</span></span>|
|<span data-ttu-id="60aab-140">windowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="60aab-140">windowsInformationProtectionPolicies</span></span>|<span data-ttu-id="60aab-141">Коллекция [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-141">[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="60aab-142">Windows Information Protection для приложений на устройствах, не зарегистрированных с использованием MDM.</span><span class="sxs-lookup"><span data-stu-id="60aab-142">Windows information protection for apps running on devices which are not MDM enrolled.</span></span>|
|<span data-ttu-id="60aab-143">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="60aab-143">managedAppRegistrations</span></span>|<span data-ttu-id="60aab-144">Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-144">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="60aab-145">Регистрации управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="60aab-145">The managed app registrations.</span></span>|
|<span data-ttu-id="60aab-146">managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="60aab-146">managedAppStatuses</span></span>|<span data-ttu-id="60aab-147">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="60aab-147">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="60aab-148">Состояния управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="60aab-148">The managed app statuses.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60aab-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60aab-149">JSON Representation</span></span>
<span data-ttu-id="60aab-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60aab-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




