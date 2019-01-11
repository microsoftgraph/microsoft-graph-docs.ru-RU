---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbc52cfd4e14b2010dd133e4fa08e61a30fb63df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814114"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="f316d-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="f316d-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="f316d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f316d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f316d-105">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="f316d-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="f316d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f316d-106">Properties</span></span>
|<span data-ttu-id="f316d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f316d-107">Property</span></span>|<span data-ttu-id="f316d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f316d-108">Type</span></span>|<span data-ttu-id="f316d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f316d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f316d-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="f316d-110">supportsUserLicensing</span></span>|<span data-ttu-id="f316d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="f316d-111">Boolean</span></span>|<span data-ttu-id="f316d-112">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="f316d-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="f316d-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="f316d-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="f316d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f316d-114">Boolean</span></span>|<span data-ttu-id="f316d-115">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="f316d-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f316d-116">Связи</span><span class="sxs-lookup"><span data-stu-id="f316d-116">Relationships</span></span>
<span data-ttu-id="f316d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f316d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f316d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f316d-118">JSON Representation</span></span>
<span data-ttu-id="f316d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f316d-119">Here is a JSON representation of the resource.</span></span>
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



