---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 121e297355d0d5734f7c4e23087bf14773c598c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553066"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="2370a-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2370a-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="2370a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2370a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2370a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2370a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2370a-106">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="2370a-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="2370a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2370a-107">Properties</span></span>
|<span data-ttu-id="2370a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2370a-108">Property</span></span>|<span data-ttu-id="2370a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2370a-109">Type</span></span>|<span data-ttu-id="2370a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2370a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2370a-111">iPad</span><span class="sxs-lookup"><span data-stu-id="2370a-111">iPad</span></span>|<span data-ttu-id="2370a-112">Логический</span><span class="sxs-lookup"><span data-stu-id="2370a-112">Boolean</span></span>|<span data-ttu-id="2370a-113">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="2370a-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="2370a-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="2370a-114">iPhoneAndIPod</span></span>|<span data-ttu-id="2370a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2370a-115">Boolean</span></span>|<span data-ttu-id="2370a-116">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="2370a-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2370a-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="2370a-117">Relationships</span></span>
<span data-ttu-id="2370a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="2370a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2370a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2370a-119">JSON Representation</span></span>
<span data-ttu-id="2370a-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2370a-120">Here is a JSON representation of the resource.</span></span>
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





