---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df465172d02b701b8b9f9439a32644f5df541f45
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448146"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="19441-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="19441-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="19441-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="19441-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19441-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19441-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19441-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="19441-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="19441-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="19441-107">Properties</span></span>
|<span data-ttu-id="19441-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="19441-108">Property</span></span>|<span data-ttu-id="19441-109">Тип</span><span class="sxs-lookup"><span data-stu-id="19441-109">Type</span></span>|<span data-ttu-id="19441-110">Описание</span><span class="sxs-lookup"><span data-stu-id="19441-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19441-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="19441-111">platformBlocked</span></span>|<span data-ttu-id="19441-112">Логический</span><span class="sxs-lookup"><span data-stu-id="19441-112">Boolean</span></span>|<span data-ttu-id="19441-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="19441-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="19441-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="19441-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="19441-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="19441-115">Boolean</span></span>|<span data-ttu-id="19441-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="19441-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="19441-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="19441-117">osMinimumVersion</span></span>|<span data-ttu-id="19441-118">String</span><span class="sxs-lookup"><span data-stu-id="19441-118">String</span></span>|<span data-ttu-id="19441-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="19441-119">Min OS version supported</span></span>|
|<span data-ttu-id="19441-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="19441-120">osMaximumVersion</span></span>|<span data-ttu-id="19441-121">String</span><span class="sxs-lookup"><span data-stu-id="19441-121">String</span></span>|<span data-ttu-id="19441-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="19441-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="19441-123">Связи</span><span class="sxs-lookup"><span data-stu-id="19441-123">Relationships</span></span>
<span data-ttu-id="19441-124">Нет</span><span class="sxs-lookup"><span data-stu-id="19441-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19441-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19441-125">JSON Representation</span></span>
<span data-ttu-id="19441-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19441-126">Here is a JSON representation of the resource.</span></span>
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




