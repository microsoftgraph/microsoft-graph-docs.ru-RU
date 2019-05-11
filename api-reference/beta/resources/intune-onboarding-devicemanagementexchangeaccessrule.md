---
title: Тип ресурса Девицеманажементексчанжеакцессруле
description: Правила доступа к устройству в Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af40f1b3b0d5602c5a67a524dc7083d95681b988
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940402"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="a3a46-103">Тип ресурса Девицеманажементексчанжеакцессруле</span><span class="sxs-lookup"><span data-stu-id="a3a46-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="a3a46-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3a46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3a46-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3a46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3a46-106">Правила доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3a46-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="a3a46-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3a46-107">Properties</span></span>
|<span data-ttu-id="a3a46-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3a46-108">Property</span></span>|<span data-ttu-id="a3a46-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a3a46-109">Type</span></span>|<span data-ttu-id="a3a46-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3a46-111">Девицекласс</span><span class="sxs-lookup"><span data-stu-id="a3a46-111">deviceClass</span></span>|[<span data-ttu-id="a3a46-112">Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="a3a46-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="a3a46-113">Класс устройства, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="a3a46-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="a3a46-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="a3a46-114">accessLevel</span></span>|[<span data-ttu-id="a3a46-115">Девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="a3a46-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="a3a46-116">Уровень доступа для Exchange, предоставляемый этим правилом.</span><span class="sxs-lookup"><span data-stu-id="a3a46-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="a3a46-117">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="a3a46-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3a46-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a3a46-118">Relationships</span></span>
<span data-ttu-id="a3a46-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a3a46-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3a46-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3a46-120">JSON Representation</span></span>
<span data-ttu-id="a3a46-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3a46-121">Here is a JSON representation of the resource.</span></span>
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




