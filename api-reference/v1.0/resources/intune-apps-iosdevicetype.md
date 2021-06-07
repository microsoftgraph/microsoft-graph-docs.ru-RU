---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 522ca687f9169066575d1bd8fb3db1e4345d9981
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755604"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="e8acd-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e8acd-103">iosDeviceType resource type</span></span>

<span data-ttu-id="e8acd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8acd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8acd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8acd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8acd-106">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="e8acd-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="e8acd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8acd-107">Properties</span></span>
|<span data-ttu-id="e8acd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8acd-108">Property</span></span>|<span data-ttu-id="e8acd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e8acd-109">Type</span></span>|<span data-ttu-id="e8acd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e8acd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8acd-111">iPad</span><span class="sxs-lookup"><span data-stu-id="e8acd-111">iPad</span></span>|<span data-ttu-id="e8acd-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8acd-112">Boolean</span></span>|<span data-ttu-id="e8acd-113">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="e8acd-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="e8acd-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="e8acd-114">iPhoneAndIPod</span></span>|<span data-ttu-id="e8acd-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8acd-115">Boolean</span></span>|<span data-ttu-id="e8acd-116">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="e8acd-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8acd-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="e8acd-117">Relationships</span></span>
<span data-ttu-id="e8acd-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e8acd-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8acd-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8acd-119">JSON Representation</span></span>
<span data-ttu-id="e8acd-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8acd-120">Here is a JSON representation of the resource.</span></span>
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




