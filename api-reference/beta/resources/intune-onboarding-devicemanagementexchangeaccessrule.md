---
title: Тип ресурса Девицеманажементексчанжеакцессруле
description: Правила доступа к устройству в Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d435d699b2cd30617a9e709ef8e9ba86eabd46b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010793"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="bd7c4-103">Тип ресурса Девицеманажементексчанжеакцессруле</span><span class="sxs-lookup"><span data-stu-id="bd7c4-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="bd7c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd7c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd7c4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd7c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd7c4-106">Правила доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd7c4-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="bd7c4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd7c4-107">Properties</span></span>
|<span data-ttu-id="bd7c4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd7c4-108">Property</span></span>|<span data-ttu-id="bd7c4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bd7c4-109">Type</span></span>|<span data-ttu-id="bd7c4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bd7c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd7c4-111">Девицекласс</span><span class="sxs-lookup"><span data-stu-id="bd7c4-111">deviceClass</span></span>|[<span data-ttu-id="bd7c4-112">Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="bd7c4-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="bd7c4-113">Класс устройства, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="bd7c4-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="bd7c4-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="bd7c4-114">accessLevel</span></span>|[<span data-ttu-id="bd7c4-115">Девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="bd7c4-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="bd7c4-116">Уровень доступа для Exchange, предоставляемый этим правилом.</span><span class="sxs-lookup"><span data-stu-id="bd7c4-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="bd7c4-117">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="bd7c4-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd7c4-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="bd7c4-118">Relationships</span></span>
<span data-ttu-id="bd7c4-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bd7c4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd7c4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd7c4-120">JSON Representation</span></span>
<span data-ttu-id="bd7c4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd7c4-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```





