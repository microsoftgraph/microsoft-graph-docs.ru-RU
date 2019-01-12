---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b541310ced9c9aaa781077639203950d00f56f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976753"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="829c1-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="829c1-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="829c1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="829c1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="829c1-105">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="829c1-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="829c1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="829c1-106">Properties</span></span>
|<span data-ttu-id="829c1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="829c1-107">Property</span></span>|<span data-ttu-id="829c1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="829c1-108">Type</span></span>|<span data-ttu-id="829c1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="829c1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="829c1-110">iPad</span><span class="sxs-lookup"><span data-stu-id="829c1-110">iPad</span></span>|<span data-ttu-id="829c1-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="829c1-111">Boolean</span></span>|<span data-ttu-id="829c1-112">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="829c1-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="829c1-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="829c1-113">iPhoneAndIPod</span></span>|<span data-ttu-id="829c1-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="829c1-114">Boolean</span></span>|<span data-ttu-id="829c1-115">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="829c1-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="829c1-116">Связи</span><span class="sxs-lookup"><span data-stu-id="829c1-116">Relationships</span></span>
<span data-ttu-id="829c1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="829c1-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="829c1-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="829c1-118">JSON Representation</span></span>
<span data-ttu-id="829c1-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="829c1-119">Here is a JSON representation of the resource.</span></span>
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



