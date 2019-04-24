---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f3bd1d0aff7e09d5828496de348805075d0b330
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503529"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="ab5c8-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ab5c8-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="ab5c8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab5c8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab5c8-105">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="ab5c8-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="ab5c8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab5c8-106">Properties</span></span>
|<span data-ttu-id="ab5c8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab5c8-107">Property</span></span>|<span data-ttu-id="ab5c8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ab5c8-108">Type</span></span>|<span data-ttu-id="ab5c8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ab5c8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab5c8-110">iPad</span><span class="sxs-lookup"><span data-stu-id="ab5c8-110">iPad</span></span>|<span data-ttu-id="ab5c8-111">Логический</span><span class="sxs-lookup"><span data-stu-id="ab5c8-111">Boolean</span></span>|<span data-ttu-id="ab5c8-112">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="ab5c8-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="ab5c8-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="ab5c8-113">iPhoneAndIPod</span></span>|<span data-ttu-id="ab5c8-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab5c8-114">Boolean</span></span>|<span data-ttu-id="ab5c8-115">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="ab5c8-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab5c8-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="ab5c8-116">Relationships</span></span>
<span data-ttu-id="ab5c8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ab5c8-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab5c8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab5c8-118">JSON Representation</span></span>
<span data-ttu-id="ab5c8-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab5c8-119">Here is a JSON representation of the resource.</span></span>
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



