---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8ba3306c5a4af4dfbb8b97e4d4794b917ebbf64
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566656"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="001b2-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="001b2-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="001b2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="001b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="001b2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="001b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="001b2-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="001b2-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="001b2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="001b2-107">Properties</span></span>
|<span data-ttu-id="001b2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="001b2-108">Property</span></span>|<span data-ttu-id="001b2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="001b2-109">Type</span></span>|<span data-ttu-id="001b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="001b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="001b2-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="001b2-111">platformBlocked</span></span>|<span data-ttu-id="001b2-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="001b2-112">Boolean</span></span>|<span data-ttu-id="001b2-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="001b2-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="001b2-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="001b2-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="001b2-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="001b2-115">Boolean</span></span>|<span data-ttu-id="001b2-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="001b2-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="001b2-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="001b2-117">osMinimumVersion</span></span>|<span data-ttu-id="001b2-118">String</span><span class="sxs-lookup"><span data-stu-id="001b2-118">String</span></span>|<span data-ttu-id="001b2-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="001b2-119">Min OS version supported</span></span>|
|<span data-ttu-id="001b2-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="001b2-120">osMaximumVersion</span></span>|<span data-ttu-id="001b2-121">String</span><span class="sxs-lookup"><span data-stu-id="001b2-121">String</span></span>|<span data-ttu-id="001b2-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="001b2-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="001b2-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="001b2-123">Relationships</span></span>
<span data-ttu-id="001b2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="001b2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="001b2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="001b2-125">JSON Representation</span></span>
<span data-ttu-id="001b2-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="001b2-126">Here is a JSON representation of the resource.</span></span>
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





