---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 057de993f7e9cef948c3334b8dcb22e34f49ba23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531238"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="aecb0-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="aecb0-103">iosDeviceType resource type</span></span>

<span data-ttu-id="aecb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aecb0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aecb0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aecb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aecb0-106">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="aecb0-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="aecb0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aecb0-107">Properties</span></span>
|<span data-ttu-id="aecb0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aecb0-108">Property</span></span>|<span data-ttu-id="aecb0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aecb0-109">Type</span></span>|<span data-ttu-id="aecb0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aecb0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aecb0-111">iPad</span><span class="sxs-lookup"><span data-stu-id="aecb0-111">iPad</span></span>|<span data-ttu-id="aecb0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="aecb0-112">Boolean</span></span>|<span data-ttu-id="aecb0-113">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="aecb0-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="aecb0-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="aecb0-114">iPhoneAndIPod</span></span>|<span data-ttu-id="aecb0-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="aecb0-115">Boolean</span></span>|<span data-ttu-id="aecb0-116">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="aecb0-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aecb0-117">Связи</span><span class="sxs-lookup"><span data-stu-id="aecb0-117">Relationships</span></span>
<span data-ttu-id="aecb0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="aecb0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aecb0-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aecb0-119">JSON Representation</span></span>
<span data-ttu-id="aecb0-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aecb0-120">Here is a JSON representation of the resource.</span></span>
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




