---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1485c429594967fd3c76fc27cb89e85c84cda92
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374360"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="26ff0-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="26ff0-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="26ff0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26ff0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26ff0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26ff0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26ff0-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="26ff0-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="26ff0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="26ff0-107">Properties</span></span>
|<span data-ttu-id="26ff0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="26ff0-108">Property</span></span>|<span data-ttu-id="26ff0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="26ff0-109">Type</span></span>|<span data-ttu-id="26ff0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="26ff0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26ff0-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="26ff0-111">platformBlocked</span></span>|<span data-ttu-id="26ff0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="26ff0-112">Boolean</span></span>|<span data-ttu-id="26ff0-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="26ff0-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="26ff0-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="26ff0-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="26ff0-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="26ff0-115">Boolean</span></span>|<span data-ttu-id="26ff0-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="26ff0-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="26ff0-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="26ff0-117">osMinimumVersion</span></span>|<span data-ttu-id="26ff0-118">String</span><span class="sxs-lookup"><span data-stu-id="26ff0-118">String</span></span>|<span data-ttu-id="26ff0-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="26ff0-119">Min OS version supported</span></span>|
|<span data-ttu-id="26ff0-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="26ff0-120">osMaximumVersion</span></span>|<span data-ttu-id="26ff0-121">String</span><span class="sxs-lookup"><span data-stu-id="26ff0-121">String</span></span>|<span data-ttu-id="26ff0-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="26ff0-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="26ff0-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="26ff0-123">Relationships</span></span>
<span data-ttu-id="26ff0-124">Нет</span><span class="sxs-lookup"><span data-stu-id="26ff0-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26ff0-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26ff0-125">JSON Representation</span></span>
<span data-ttu-id="26ff0-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26ff0-126">Here is a JSON representation of the resource.</span></span>
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



