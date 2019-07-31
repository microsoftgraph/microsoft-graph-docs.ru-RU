---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d0e881053d3b24bbfa12e627a4f21ded4049747
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998193"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="75e53-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="75e53-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="75e53-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75e53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75e53-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75e53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75e53-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="75e53-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="75e53-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="75e53-107">Properties</span></span>
|<span data-ttu-id="75e53-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="75e53-108">Property</span></span>|<span data-ttu-id="75e53-109">Тип</span><span class="sxs-lookup"><span data-stu-id="75e53-109">Type</span></span>|<span data-ttu-id="75e53-110">Описание</span><span class="sxs-lookup"><span data-stu-id="75e53-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75e53-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="75e53-111">platformBlocked</span></span>|<span data-ttu-id="75e53-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="75e53-112">Boolean</span></span>|<span data-ttu-id="75e53-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="75e53-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="75e53-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="75e53-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="75e53-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="75e53-115">Boolean</span></span>|<span data-ttu-id="75e53-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="75e53-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="75e53-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="75e53-117">osMinimumVersion</span></span>|<span data-ttu-id="75e53-118">String</span><span class="sxs-lookup"><span data-stu-id="75e53-118">String</span></span>|<span data-ttu-id="75e53-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="75e53-119">Min OS version supported</span></span>|
|<span data-ttu-id="75e53-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="75e53-120">osMaximumVersion</span></span>|<span data-ttu-id="75e53-121">String</span><span class="sxs-lookup"><span data-stu-id="75e53-121">String</span></span>|<span data-ttu-id="75e53-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="75e53-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="75e53-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="75e53-123">Relationships</span></span>
<span data-ttu-id="75e53-124">Нет</span><span class="sxs-lookup"><span data-stu-id="75e53-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75e53-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75e53-125">JSON Representation</span></span>
<span data-ttu-id="75e53-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75e53-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```





