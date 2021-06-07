---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02978735f15ce036c8ffbc81340d965d67a21ce8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751617"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="cfce4-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cfce4-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="cfce4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfce4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfce4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfce4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfce4-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="cfce4-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="cfce4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfce4-107">Properties</span></span>
|<span data-ttu-id="cfce4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfce4-108">Property</span></span>|<span data-ttu-id="cfce4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cfce4-109">Type</span></span>|<span data-ttu-id="cfce4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cfce4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfce4-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="cfce4-111">platformBlocked</span></span>|<span data-ttu-id="cfce4-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfce4-112">Boolean</span></span>|<span data-ttu-id="cfce4-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="cfce4-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="cfce4-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="cfce4-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="cfce4-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfce4-115">Boolean</span></span>|<span data-ttu-id="cfce4-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="cfce4-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="cfce4-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cfce4-117">osMinimumVersion</span></span>|<span data-ttu-id="cfce4-118">String</span><span class="sxs-lookup"><span data-stu-id="cfce4-118">String</span></span>|<span data-ttu-id="cfce4-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="cfce4-119">Min OS version supported</span></span>|
|<span data-ttu-id="cfce4-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cfce4-120">osMaximumVersion</span></span>|<span data-ttu-id="cfce4-121">String</span><span class="sxs-lookup"><span data-stu-id="cfce4-121">String</span></span>|<span data-ttu-id="cfce4-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="cfce4-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfce4-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="cfce4-123">Relationships</span></span>
<span data-ttu-id="cfce4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="cfce4-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfce4-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfce4-125">JSON Representation</span></span>
<span data-ttu-id="cfce4-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfce4-126">Here is a JSON representation of the resource.</span></span>
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




