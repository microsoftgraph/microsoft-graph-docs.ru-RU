---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b68c7ce163dbf0f9232bf53d919ae84c7906c997
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395386"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="54606-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="54606-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="54606-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54606-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54606-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54606-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54606-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54606-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54606-107">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="54606-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="54606-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="54606-108">Properties</span></span>
|<span data-ttu-id="54606-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="54606-109">Property</span></span>|<span data-ttu-id="54606-110">Тип</span><span class="sxs-lookup"><span data-stu-id="54606-110">Type</span></span>|<span data-ttu-id="54606-111">Описание</span><span class="sxs-lookup"><span data-stu-id="54606-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54606-112">iPad</span><span class="sxs-lookup"><span data-stu-id="54606-112">iPad</span></span>|<span data-ttu-id="54606-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="54606-113">Boolean</span></span>|<span data-ttu-id="54606-114">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="54606-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="54606-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="54606-115">iPhoneAndIPod</span></span>|<span data-ttu-id="54606-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="54606-116">Boolean</span></span>|<span data-ttu-id="54606-117">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="54606-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54606-118">Связи</span><span class="sxs-lookup"><span data-stu-id="54606-118">Relationships</span></span>
<span data-ttu-id="54606-119">Нет</span><span class="sxs-lookup"><span data-stu-id="54606-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54606-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54606-120">JSON Representation</span></span>
<span data-ttu-id="54606-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54606-121">Here is a JSON representation of the resource.</span></span>
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




