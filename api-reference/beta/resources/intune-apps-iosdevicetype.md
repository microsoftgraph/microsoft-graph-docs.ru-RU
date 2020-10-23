---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19dc8db9f4d5a619add49e6693b97d8175c5e6da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730772"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="c6152-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="c6152-103">iosDeviceType resource type</span></span>

<span data-ttu-id="c6152-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6152-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6152-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6152-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6152-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6152-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6152-107">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="c6152-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="c6152-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6152-108">Properties</span></span>
|<span data-ttu-id="c6152-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6152-109">Property</span></span>|<span data-ttu-id="c6152-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c6152-110">Type</span></span>|<span data-ttu-id="c6152-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c6152-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6152-112">iPad</span><span class="sxs-lookup"><span data-stu-id="c6152-112">iPad</span></span>|<span data-ttu-id="c6152-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6152-113">Boolean</span></span>|<span data-ttu-id="c6152-114">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="c6152-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="c6152-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="c6152-115">iPhoneAndIPod</span></span>|<span data-ttu-id="c6152-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6152-116">Boolean</span></span>|<span data-ttu-id="c6152-117">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="c6152-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6152-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c6152-118">Relationships</span></span>
<span data-ttu-id="c6152-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c6152-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6152-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6152-120">JSON Representation</span></span>
<span data-ttu-id="c6152-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6152-121">Here is a JSON representation of the resource.</span></span>
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





