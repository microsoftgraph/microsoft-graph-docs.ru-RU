---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9c3478e7fc67f288102e313f44bf08b55e01f222
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760309"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="49a7d-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="49a7d-103">vppLicensingType resource type</span></span>

<span data-ttu-id="49a7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49a7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49a7d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49a7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49a7d-106">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="49a7d-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="49a7d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="49a7d-107">Properties</span></span>
|<span data-ttu-id="49a7d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="49a7d-108">Property</span></span>|<span data-ttu-id="49a7d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="49a7d-109">Type</span></span>|<span data-ttu-id="49a7d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="49a7d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49a7d-111">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="49a7d-111">supportsUserLicensing</span></span>|<span data-ttu-id="49a7d-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="49a7d-112">Boolean</span></span>|<span data-ttu-id="49a7d-113">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="49a7d-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="49a7d-114">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="49a7d-114">supportsDeviceLicensing</span></span>|<span data-ttu-id="49a7d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="49a7d-115">Boolean</span></span>|<span data-ttu-id="49a7d-116">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="49a7d-116">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49a7d-117">Связи</span><span class="sxs-lookup"><span data-stu-id="49a7d-117">Relationships</span></span>
<span data-ttu-id="49a7d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="49a7d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49a7d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49a7d-119">JSON Representation</span></span>
<span data-ttu-id="49a7d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49a7d-120">Here is a JSON representation of the resource.</span></span>
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




