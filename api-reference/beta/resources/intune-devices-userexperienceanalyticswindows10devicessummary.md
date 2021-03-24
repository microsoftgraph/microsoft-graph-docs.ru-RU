---
title: тип ресурса userExperienceAnalyticsWindows10DevicesSummary
description: Аналитика пользовательских интерфейсов работает из любого сводки устройств Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f43c2848902b6d9fbb3e54a2fd9a8ac36edc0793
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146830"
---
# <a name="userexperienceanalyticswindows10devicessummary-resource-type"></a><span data-ttu-id="04d2e-103">тип ресурса userExperienceAnalyticsWindows10DevicesSummary</span><span class="sxs-lookup"><span data-stu-id="04d2e-103">userExperienceAnalyticsWindows10DevicesSummary resource type</span></span>

<span data-ttu-id="04d2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04d2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04d2e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04d2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04d2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04d2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04d2e-107">Аналитика пользовательских интерфейсов работает из любого сводки устройств Windows 10.</span><span class="sxs-lookup"><span data-stu-id="04d2e-107">The user experience analytics work from anywhere Windows 10 devices summary.</span></span>

## <a name="properties"></a><span data-ttu-id="04d2e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="04d2e-108">Properties</span></span>
|<span data-ttu-id="04d2e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="04d2e-109">Property</span></span>|<span data-ttu-id="04d2e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="04d2e-110">Type</span></span>|<span data-ttu-id="04d2e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="04d2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04d2e-112">unsupportedOSversionDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04d2e-112">unsupportedOSversionDeviceCount</span></span>|<span data-ttu-id="04d2e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="04d2e-113">Int32</span></span>|<span data-ttu-id="04d2e-114">Количество устройств с Windows 10 с неподтверченными версиями ОС.</span><span class="sxs-lookup"><span data-stu-id="04d2e-114">The count of Windows 10 devices that have unsupported OS versions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04d2e-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="04d2e-115">Relationships</span></span>
<span data-ttu-id="04d2e-116">Нет</span><span class="sxs-lookup"><span data-stu-id="04d2e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04d2e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04d2e-117">JSON Representation</span></span>
<span data-ttu-id="04d2e-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04d2e-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
  "unsupportedOSversionDeviceCount": 1024
}
```




