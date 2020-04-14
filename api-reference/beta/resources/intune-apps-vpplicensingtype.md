---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f31388de57835ea91ae3dc9fd104dd3b74b0ae32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43362767"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="a00d2-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="a00d2-103">vppLicensingType resource type</span></span>

<span data-ttu-id="a00d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a00d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a00d2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a00d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a00d2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a00d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a00d2-107">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="a00d2-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="a00d2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a00d2-108">Properties</span></span>
|<span data-ttu-id="a00d2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a00d2-109">Property</span></span>|<span data-ttu-id="a00d2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a00d2-110">Type</span></span>|<span data-ttu-id="a00d2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a00d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a00d2-112">суппортусерлиценсинг</span><span class="sxs-lookup"><span data-stu-id="a00d2-112">supportUserLicensing</span></span>|<span data-ttu-id="a00d2-113">Логическое</span><span class="sxs-lookup"><span data-stu-id="a00d2-113">Boolean</span></span>|<span data-ttu-id="a00d2-114">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="a00d2-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="a00d2-115">суппортдевицелиценсинг</span><span class="sxs-lookup"><span data-stu-id="a00d2-115">supportDeviceLicensing</span></span>|<span data-ttu-id="a00d2-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a00d2-116">Boolean</span></span>|<span data-ttu-id="a00d2-117">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="a00d2-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="a00d2-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="a00d2-118">supportsUserLicensing</span></span>|<span data-ttu-id="a00d2-119">Логическое</span><span class="sxs-lookup"><span data-stu-id="a00d2-119">Boolean</span></span>|<span data-ttu-id="a00d2-120">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="a00d2-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="a00d2-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a00d2-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="a00d2-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="a00d2-122">Boolean</span></span>|<span data-ttu-id="a00d2-123">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="a00d2-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a00d2-124">Связи</span><span class="sxs-lookup"><span data-stu-id="a00d2-124">Relationships</span></span>
<span data-ttu-id="a00d2-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a00d2-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a00d2-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a00d2-126">JSON Representation</span></span>
<span data-ttu-id="a00d2-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a00d2-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



