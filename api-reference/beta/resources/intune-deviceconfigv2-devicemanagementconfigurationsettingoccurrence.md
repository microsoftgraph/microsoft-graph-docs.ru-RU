---
title: Тип ресурса Девицеманажементконфигуратионсеттингоккурренце
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b8a93c75f011dba9816ee84a9ef8bf5cd05d275
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302207"
---
# <a name="devicemanagementconfigurationsettingoccurrence-resource-type"></a><span data-ttu-id="9480a-103">Тип ресурса Девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="9480a-103">deviceManagementConfigurationSettingOccurrence resource type</span></span>

<span data-ttu-id="9480a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9480a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9480a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9480a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9480a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9480a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9480a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9480a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9480a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9480a-108">Properties</span></span>
|<span data-ttu-id="9480a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9480a-109">Property</span></span>|<span data-ttu-id="9480a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9480a-110">Type</span></span>|<span data-ttu-id="9480a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9480a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9480a-112">миндевицеоккурренце</span><span class="sxs-lookup"><span data-stu-id="9480a-112">minDeviceOccurrence</span></span>|<span data-ttu-id="9480a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9480a-113">Int32</span></span>|<span data-ttu-id="9480a-114">Параметр минимальной настройки можно задать для устройства.</span><span class="sxs-lookup"><span data-stu-id="9480a-114">Minimum times setting can be set on device.</span></span> <span data-ttu-id="9480a-115">Миндевицеоккурренце 0 означает, что параметр является необязательным</span><span class="sxs-lookup"><span data-stu-id="9480a-115">A MinDeviceOccurrence of 0 means setting is optional</span></span>|
|<span data-ttu-id="9480a-116">максдевицеоккурренце</span><span class="sxs-lookup"><span data-stu-id="9480a-116">maxDeviceOccurrence</span></span>|<span data-ttu-id="9480a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="9480a-117">Int32</span></span>|<span data-ttu-id="9480a-118">Параметр максимальных значений времени можно задать для устройства.</span><span class="sxs-lookup"><span data-stu-id="9480a-118">Maximum times setting can be set on device.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9480a-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9480a-119">Relationships</span></span>
<span data-ttu-id="9480a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9480a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9480a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9480a-121">JSON Representation</span></span>
<span data-ttu-id="9480a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9480a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingOccurrence",
  "minDeviceOccurrence": 1024,
  "maxDeviceOccurrence": 1024
}
```




