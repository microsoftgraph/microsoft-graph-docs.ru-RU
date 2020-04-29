---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df7d130b1ee3354a0a82788ce58543b9eb6e7896
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439647"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="eef3c-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="eef3c-103">vppLicensingType resource type</span></span>

<span data-ttu-id="eef3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef3c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eef3c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eef3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eef3c-106">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="eef3c-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="eef3c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eef3c-107">Properties</span></span>
|<span data-ttu-id="eef3c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eef3c-108">Property</span></span>|<span data-ttu-id="eef3c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eef3c-109">Type</span></span>|<span data-ttu-id="eef3c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eef3c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef3c-111">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="eef3c-111">supportsUserLicensing</span></span>|<span data-ttu-id="eef3c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="eef3c-112">Boolean</span></span>|<span data-ttu-id="eef3c-113">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="eef3c-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="eef3c-114">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="eef3c-114">supportsDeviceLicensing</span></span>|<span data-ttu-id="eef3c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="eef3c-115">Boolean</span></span>|<span data-ttu-id="eef3c-116">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="eef3c-116">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eef3c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="eef3c-117">Relationships</span></span>
<span data-ttu-id="eef3c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="eef3c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eef3c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eef3c-119">JSON Representation</span></span>
<span data-ttu-id="eef3c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eef3c-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```







