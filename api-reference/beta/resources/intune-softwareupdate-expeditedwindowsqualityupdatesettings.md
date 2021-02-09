---
title: Тип ресурса expeditedWindowsQualityUpdateSettings
description: Сложный тип для хранения параметров автоматического обновления качества, таких как дата и дни выпуска до принудительной перезагрузки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 700b86d15737c75cbf10679ea6e944726d667431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160610"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a><span data-ttu-id="3d284-103">Тип ресурса expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="3d284-103">expeditedWindowsQualityUpdateSettings resource type</span></span>

<span data-ttu-id="3d284-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d284-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d284-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d284-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d284-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d284-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d284-107">Сложный тип для хранения параметров автоматического обновления качества, таких как дата выпуска и дни до принудительной перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="3d284-107">A complex type to store the expedited quality update settings such as release date and days until forced reboot.</span></span>

## <a name="properties"></a><span data-ttu-id="3d284-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d284-108">Properties</span></span>
|<span data-ttu-id="3d284-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d284-109">Property</span></span>|<span data-ttu-id="3d284-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3d284-110">Type</span></span>|<span data-ttu-id="3d284-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3d284-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d284-112">qualityUpdateRelease</span><span class="sxs-lookup"><span data-stu-id="3d284-112">qualityUpdateRelease</span></span>|<span data-ttu-id="3d284-113">String</span><span class="sxs-lookup"><span data-stu-id="3d284-113">String</span></span>|<span data-ttu-id="3d284-114">Дата выпуска для определения обновления качества.</span><span class="sxs-lookup"><span data-stu-id="3d284-114">The release date to identify a quality update.</span></span>|
|<span data-ttu-id="3d284-115">daysUntilForcedReboot</span><span class="sxs-lookup"><span data-stu-id="3d284-115">daysUntilForcedReboot</span></span>|<span data-ttu-id="3d284-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3d284-116">Int32</span></span>|<span data-ttu-id="3d284-117">Количество дней после установки, в течение чего произойдет принудительный перезагруза.</span><span class="sxs-lookup"><span data-stu-id="3d284-117">The number of days after installation that forced reboot will happen.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d284-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3d284-118">Relationships</span></span>
<span data-ttu-id="3d284-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3d284-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d284-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d284-120">JSON Representation</span></span>
<span data-ttu-id="3d284-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d284-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expeditedWindowsQualityUpdateSettings",
  "qualityUpdateRelease": "String",
  "daysUntilForcedReboot": 1024
}
```




