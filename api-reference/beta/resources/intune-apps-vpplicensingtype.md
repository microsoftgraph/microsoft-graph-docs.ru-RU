---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 47ee634c8fa488bb27c6c0a4beb7728fc7e427cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948683"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="b6687-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="b6687-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="b6687-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6687-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6687-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6687-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6687-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6687-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6687-107">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="b6687-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="b6687-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6687-108">Properties</span></span>
|<span data-ttu-id="b6687-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6687-109">Property</span></span>|<span data-ttu-id="b6687-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b6687-110">Type</span></span>|<span data-ttu-id="b6687-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6687-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6687-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="b6687-112">supportUserLicensing</span></span>|<span data-ttu-id="b6687-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6687-113">Boolean</span></span>|<span data-ttu-id="b6687-114">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6687-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="b6687-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="b6687-115">supportDeviceLicensing</span></span>|<span data-ttu-id="b6687-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6687-116">Boolean</span></span>|<span data-ttu-id="b6687-117">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="b6687-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="b6687-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="b6687-118">supportsUserLicensing</span></span>|<span data-ttu-id="b6687-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6687-119">Boolean</span></span>|<span data-ttu-id="b6687-120">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6687-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="b6687-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="b6687-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="b6687-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6687-122">Boolean</span></span>|<span data-ttu-id="b6687-123">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="b6687-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6687-124">Связи</span><span class="sxs-lookup"><span data-stu-id="b6687-124">Relationships</span></span>
<span data-ttu-id="b6687-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b6687-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b6687-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6687-126">JSON Representation</span></span>
<span data-ttu-id="b6687-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6687-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





