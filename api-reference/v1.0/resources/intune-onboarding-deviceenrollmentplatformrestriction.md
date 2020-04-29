---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 248127b41ca999ceba27f077391a7afa3f4bfbae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459560"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="39907-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="39907-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="39907-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39907-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39907-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39907-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39907-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="39907-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="39907-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="39907-107">Properties</span></span>
|<span data-ttu-id="39907-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="39907-108">Property</span></span>|<span data-ttu-id="39907-109">Тип</span><span class="sxs-lookup"><span data-stu-id="39907-109">Type</span></span>|<span data-ttu-id="39907-110">Описание</span><span class="sxs-lookup"><span data-stu-id="39907-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39907-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="39907-111">platformBlocked</span></span>|<span data-ttu-id="39907-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="39907-112">Boolean</span></span>|<span data-ttu-id="39907-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="39907-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="39907-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="39907-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="39907-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="39907-115">Boolean</span></span>|<span data-ttu-id="39907-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="39907-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="39907-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="39907-117">osMinimumVersion</span></span>|<span data-ttu-id="39907-118">String</span><span class="sxs-lookup"><span data-stu-id="39907-118">String</span></span>|<span data-ttu-id="39907-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="39907-119">Min OS version supported</span></span>|
|<span data-ttu-id="39907-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="39907-120">osMaximumVersion</span></span>|<span data-ttu-id="39907-121">String</span><span class="sxs-lookup"><span data-stu-id="39907-121">String</span></span>|<span data-ttu-id="39907-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="39907-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="39907-123">Связи</span><span class="sxs-lookup"><span data-stu-id="39907-123">Relationships</span></span>
<span data-ttu-id="39907-124">Нет</span><span class="sxs-lookup"><span data-stu-id="39907-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39907-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39907-125">JSON Representation</span></span>
<span data-ttu-id="39907-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39907-126">Here is a JSON representation of the resource.</span></span>
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







