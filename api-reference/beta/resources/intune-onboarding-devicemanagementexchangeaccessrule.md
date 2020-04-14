---
title: Тип ресурса Девицеманажементексчанжеакцессруле
description: Правила доступа к устройству в Exchange.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: afe7cde845bfff01100f5e8fabea22d6ce863f63
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455041"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="b17bd-103">Тип ресурса Девицеманажементексчанжеакцессруле</span><span class="sxs-lookup"><span data-stu-id="b17bd-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="b17bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b17bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b17bd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b17bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b17bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b17bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b17bd-107">Правила доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b17bd-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="b17bd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b17bd-108">Properties</span></span>
|<span data-ttu-id="b17bd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b17bd-109">Property</span></span>|<span data-ttu-id="b17bd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b17bd-110">Type</span></span>|<span data-ttu-id="b17bd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b17bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b17bd-112">девицекласс</span><span class="sxs-lookup"><span data-stu-id="b17bd-112">deviceClass</span></span>|[<span data-ttu-id="b17bd-113">девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="b17bd-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="b17bd-114">Класс устройства, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="b17bd-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="b17bd-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="b17bd-115">accessLevel</span></span>|[<span data-ttu-id="b17bd-116">девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="b17bd-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="b17bd-117">Уровень доступа для Exchange, предоставляемый этим правилом.</span><span class="sxs-lookup"><span data-stu-id="b17bd-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="b17bd-118">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="b17bd-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b17bd-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b17bd-119">Relationships</span></span>
<span data-ttu-id="b17bd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b17bd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b17bd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b17bd-121">JSON Representation</span></span>
<span data-ttu-id="b17bd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b17bd-122">Here is a JSON representation of the resource.</span></span>
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



