---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 587c5e319490807369590585e53a06e0dcc7f2bb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37369060"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="0ed7a-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="0ed7a-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="0ed7a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ed7a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ed7a-105">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="0ed7a-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="0ed7a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ed7a-106">Properties</span></span>
|<span data-ttu-id="0ed7a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ed7a-107">Property</span></span>|<span data-ttu-id="0ed7a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0ed7a-108">Type</span></span>|<span data-ttu-id="0ed7a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0ed7a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ed7a-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="0ed7a-110">supportsUserLicensing</span></span>|<span data-ttu-id="0ed7a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ed7a-111">Boolean</span></span>|<span data-ttu-id="0ed7a-112">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="0ed7a-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="0ed7a-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="0ed7a-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="0ed7a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ed7a-114">Boolean</span></span>|<span data-ttu-id="0ed7a-115">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="0ed7a-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ed7a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="0ed7a-116">Relationships</span></span>
<span data-ttu-id="0ed7a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0ed7a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ed7a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ed7a-118">JSON Representation</span></span>
<span data-ttu-id="0ed7a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ed7a-119">Here is a JSON representation of the resource.</span></span>
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




