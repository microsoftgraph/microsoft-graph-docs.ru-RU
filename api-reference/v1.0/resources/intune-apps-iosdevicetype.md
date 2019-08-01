---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23d38faeafd9aac0d0e547596de51507b6932c20
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029166"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="1af0a-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1af0a-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="1af0a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1af0a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af0a-105">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="1af0a-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="1af0a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1af0a-106">Properties</span></span>
|<span data-ttu-id="1af0a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1af0a-107">Property</span></span>|<span data-ttu-id="1af0a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1af0a-108">Type</span></span>|<span data-ttu-id="1af0a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1af0a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af0a-110">iPad</span><span class="sxs-lookup"><span data-stu-id="1af0a-110">iPad</span></span>|<span data-ttu-id="1af0a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1af0a-111">Boolean</span></span>|<span data-ttu-id="1af0a-112">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="1af0a-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="1af0a-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="1af0a-113">iPhoneAndIPod</span></span>|<span data-ttu-id="1af0a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1af0a-114">Boolean</span></span>|<span data-ttu-id="1af0a-115">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="1af0a-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1af0a-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="1af0a-116">Relationships</span></span>
<span data-ttu-id="1af0a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1af0a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1af0a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1af0a-118">JSON Representation</span></span>
<span data-ttu-id="1af0a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1af0a-119">Here is a JSON representation of the resource.</span></span>
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



