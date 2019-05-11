---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 660265882a0b40e365dc49b0642f078ac4df73ea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950398"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="502db-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="502db-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="502db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="502db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="502db-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="502db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="502db-106">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="502db-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="502db-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="502db-107">Properties</span></span>
|<span data-ttu-id="502db-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="502db-108">Property</span></span>|<span data-ttu-id="502db-109">Тип</span><span class="sxs-lookup"><span data-stu-id="502db-109">Type</span></span>|<span data-ttu-id="502db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="502db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="502db-111">iPad</span><span class="sxs-lookup"><span data-stu-id="502db-111">iPad</span></span>|<span data-ttu-id="502db-112">Логический</span><span class="sxs-lookup"><span data-stu-id="502db-112">Boolean</span></span>|<span data-ttu-id="502db-113">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="502db-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="502db-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="502db-114">iPhoneAndIPod</span></span>|<span data-ttu-id="502db-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="502db-115">Boolean</span></span>|<span data-ttu-id="502db-116">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="502db-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="502db-117">Связи</span><span class="sxs-lookup"><span data-stu-id="502db-117">Relationships</span></span>
<span data-ttu-id="502db-118">Нет</span><span class="sxs-lookup"><span data-stu-id="502db-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="502db-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="502db-119">JSON Representation</span></span>
<span data-ttu-id="502db-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="502db-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```




