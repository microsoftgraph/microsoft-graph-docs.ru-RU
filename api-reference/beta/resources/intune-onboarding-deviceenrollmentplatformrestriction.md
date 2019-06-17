---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0288883ec1deaaecc142aec42f413a4f60a76b5b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993160"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="63dce-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63dce-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="63dce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63dce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63dce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63dce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63dce-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="63dce-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="63dce-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="63dce-107">Properties</span></span>
|<span data-ttu-id="63dce-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="63dce-108">Property</span></span>|<span data-ttu-id="63dce-109">Тип</span><span class="sxs-lookup"><span data-stu-id="63dce-109">Type</span></span>|<span data-ttu-id="63dce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="63dce-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63dce-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="63dce-111">platformBlocked</span></span>|<span data-ttu-id="63dce-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="63dce-112">Boolean</span></span>|<span data-ttu-id="63dce-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="63dce-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="63dce-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="63dce-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="63dce-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="63dce-115">Boolean</span></span>|<span data-ttu-id="63dce-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="63dce-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="63dce-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="63dce-117">osMinimumVersion</span></span>|<span data-ttu-id="63dce-118">String</span><span class="sxs-lookup"><span data-stu-id="63dce-118">String</span></span>|<span data-ttu-id="63dce-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="63dce-119">Min OS version supported</span></span>|
|<span data-ttu-id="63dce-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="63dce-120">osMaximumVersion</span></span>|<span data-ttu-id="63dce-121">String</span><span class="sxs-lookup"><span data-stu-id="63dce-121">String</span></span>|<span data-ttu-id="63dce-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="63dce-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="63dce-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="63dce-123">Relationships</span></span>
<span data-ttu-id="63dce-124">Нет</span><span class="sxs-lookup"><span data-stu-id="63dce-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63dce-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63dce-125">JSON Representation</span></span>
<span data-ttu-id="63dce-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63dce-126">Here is a JSON representation of the resource.</span></span>
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





