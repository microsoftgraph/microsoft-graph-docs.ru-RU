---
title: тип ресурса userExperienceSettings
description: Параметры управлять опытом обновления пользователя на устройстве.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a5d920d1618cb6d212baf0487a39960638859cef
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067483"
---
# <a name="userexperiencesettings-resource-type"></a><span data-ttu-id="7d2cb-103">тип ресурса userExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="7d2cb-103">userExperienceSettings resource type</span></span>

<span data-ttu-id="7d2cb-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="7d2cb-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d2cb-105">Параметры управлять опытом обновления пользователя на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7d2cb-105">Settings controlling the user's update experience on a device.</span></span>

## <a name="properties"></a><span data-ttu-id="7d2cb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d2cb-106">Properties</span></span>
|<span data-ttu-id="7d2cb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d2cb-107">Property</span></span>|<span data-ttu-id="7d2cb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7d2cb-108">Type</span></span>|<span data-ttu-id="7d2cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d2cb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d2cb-110">daysUntilForcedReboot</span><span class="sxs-lookup"><span data-stu-id="7d2cb-110">daysUntilForcedReboot</span></span>|<span data-ttu-id="7d2cb-111">Int32</span><span class="sxs-lookup"><span data-stu-id="7d2cb-111">Int32</span></span>|<span data-ttu-id="7d2cb-112">Указывает количество дней после установки обновления, в течение которых пользователь устройства может управлять при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="7d2cb-112">Specifies the number of days after an update is installed, during which the user of the device can control when the device restarts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d2cb-113">Связи</span><span class="sxs-lookup"><span data-stu-id="7d2cb-113">Relationships</span></span>
<span data-ttu-id="7d2cb-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7d2cb-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d2cb-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7d2cb-115">JSON representation</span></span>
<span data-ttu-id="7d2cb-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d2cb-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.userExperienceSettings",
  "daysUntilForcedReboot": "Integer"
}
```

