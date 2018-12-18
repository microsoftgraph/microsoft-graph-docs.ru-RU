---
title: Тип ресурса operatingSystemVersionRange
description: Диапазон версии операционной системы.
author: tfitzmac
ms.openlocfilehash: b853e71b2d8f66d24122afb51cea97fc6a8f8d7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331166"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="66854-103">Тип ресурса operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="66854-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="66854-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66854-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66854-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66854-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66854-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="66854-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66854-107">Диапазон версии операционной системы.</span><span class="sxs-lookup"><span data-stu-id="66854-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="66854-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="66854-108">Properties</span></span>
|<span data-ttu-id="66854-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="66854-109">Property</span></span>|<span data-ttu-id="66854-110">Тип</span><span class="sxs-lookup"><span data-stu-id="66854-110">Type</span></span>|<span data-ttu-id="66854-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66854-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66854-112">описание</span><span class="sxs-lookup"><span data-stu-id="66854-112">description</span></span>|<span data-ttu-id="66854-113">Строка</span><span class="sxs-lookup"><span data-stu-id="66854-113">String</span></span>|<span data-ttu-id="66854-114">Описание этого диапазона (например действительно 1702 сборок)</span><span class="sxs-lookup"><span data-stu-id="66854-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="66854-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="66854-115">lowestVersion</span></span>|<span data-ttu-id="66854-116">String.</span><span class="sxs-lookup"><span data-stu-id="66854-116">String</span></span>|<span data-ttu-id="66854-117">Низший включительно версия, которая содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="66854-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="66854-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="66854-118">highestVersion</span></span>|<span data-ttu-id="66854-119">String.</span><span class="sxs-lookup"><span data-stu-id="66854-119">String</span></span>|<span data-ttu-id="66854-120">Наибольший включительно версию, которая содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="66854-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66854-121">Связи</span><span class="sxs-lookup"><span data-stu-id="66854-121">Relationships</span></span>
<span data-ttu-id="66854-122">Нет</span><span class="sxs-lookup"><span data-stu-id="66854-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66854-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66854-123">JSON Representation</span></span>
<span data-ttu-id="66854-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66854-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





