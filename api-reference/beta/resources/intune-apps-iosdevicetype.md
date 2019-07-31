---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a28f426199280c98ceadd31560b22fa48829d969
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005550"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="5ee15-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5ee15-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="5ee15-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ee15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ee15-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ee15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee15-106">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="5ee15-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="5ee15-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ee15-107">Properties</span></span>
|<span data-ttu-id="5ee15-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ee15-108">Property</span></span>|<span data-ttu-id="5ee15-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5ee15-109">Type</span></span>|<span data-ttu-id="5ee15-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5ee15-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee15-111">iPad</span><span class="sxs-lookup"><span data-stu-id="5ee15-111">iPad</span></span>|<span data-ttu-id="5ee15-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee15-112">Boolean</span></span>|<span data-ttu-id="5ee15-113">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="5ee15-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="5ee15-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="5ee15-114">iPhoneAndIPod</span></span>|<span data-ttu-id="5ee15-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee15-115">Boolean</span></span>|<span data-ttu-id="5ee15-116">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="5ee15-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ee15-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="5ee15-117">Relationships</span></span>
<span data-ttu-id="5ee15-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5ee15-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ee15-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ee15-119">JSON Representation</span></span>
<span data-ttu-id="5ee15-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ee15-120">Here is a JSON representation of the resource.</span></span>
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





