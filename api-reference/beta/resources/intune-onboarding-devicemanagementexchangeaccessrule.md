---
title: Тип ресурса Девицеманажементексчанжеакцессруле
description: Правила доступа к устройству в Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 832e11829300ccd1ac4e1d4e6b08acafb908f3b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566607"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="221a5-103">Тип ресурса Девицеманажементексчанжеакцессруле</span><span class="sxs-lookup"><span data-stu-id="221a5-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="221a5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="221a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="221a5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="221a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="221a5-106">Правила доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="221a5-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="221a5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="221a5-107">Properties</span></span>
|<span data-ttu-id="221a5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="221a5-108">Property</span></span>|<span data-ttu-id="221a5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="221a5-109">Type</span></span>|<span data-ttu-id="221a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="221a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="221a5-111">Девицекласс</span><span class="sxs-lookup"><span data-stu-id="221a5-111">deviceClass</span></span>|[<span data-ttu-id="221a5-112">Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="221a5-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="221a5-113">Класс устройства, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="221a5-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="221a5-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="221a5-114">accessLevel</span></span>|[<span data-ttu-id="221a5-115">Девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="221a5-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="221a5-116">Уровень доступа для Exchange, предоставляемый этим правилом.</span><span class="sxs-lookup"><span data-stu-id="221a5-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="221a5-117">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="221a5-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="221a5-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="221a5-118">Relationships</span></span>
<span data-ttu-id="221a5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="221a5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="221a5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="221a5-120">JSON Representation</span></span>
<span data-ttu-id="221a5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="221a5-121">Here is a JSON representation of the resource.</span></span>
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





