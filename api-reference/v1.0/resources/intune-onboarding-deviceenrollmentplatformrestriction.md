---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c621eb9fc0b90e752d46b8ab1a3d75a927c16051
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086551"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="07ae2-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="07ae2-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="07ae2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07ae2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07ae2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07ae2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07ae2-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="07ae2-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="07ae2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="07ae2-107">Properties</span></span>
|<span data-ttu-id="07ae2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="07ae2-108">Property</span></span>|<span data-ttu-id="07ae2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="07ae2-109">Type</span></span>|<span data-ttu-id="07ae2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07ae2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07ae2-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="07ae2-111">platformBlocked</span></span>|<span data-ttu-id="07ae2-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="07ae2-112">Boolean</span></span>|<span data-ttu-id="07ae2-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="07ae2-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="07ae2-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="07ae2-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="07ae2-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="07ae2-115">Boolean</span></span>|<span data-ttu-id="07ae2-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="07ae2-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="07ae2-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="07ae2-117">osMinimumVersion</span></span>|<span data-ttu-id="07ae2-118">String</span><span class="sxs-lookup"><span data-stu-id="07ae2-118">String</span></span>|<span data-ttu-id="07ae2-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="07ae2-119">Min OS version supported</span></span>|
|<span data-ttu-id="07ae2-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="07ae2-120">osMaximumVersion</span></span>|<span data-ttu-id="07ae2-121">String</span><span class="sxs-lookup"><span data-stu-id="07ae2-121">String</span></span>|<span data-ttu-id="07ae2-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="07ae2-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="07ae2-123">Связи</span><span class="sxs-lookup"><span data-stu-id="07ae2-123">Relationships</span></span>
<span data-ttu-id="07ae2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="07ae2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07ae2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07ae2-125">JSON Representation</span></span>
<span data-ttu-id="07ae2-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07ae2-126">Here is a JSON representation of the resource.</span></span>
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









