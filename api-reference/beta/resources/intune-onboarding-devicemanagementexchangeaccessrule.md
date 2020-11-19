---
title: Тип ресурса Девицеманажементексчанжеакцессруле
description: Правила доступа к устройству в Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ecd6777327defe913818e984ca30d2bc6f47157
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307425"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="d42c2-103">Тип ресурса Девицеманажементексчанжеакцессруле</span><span class="sxs-lookup"><span data-stu-id="d42c2-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="d42c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d42c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d42c2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d42c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d42c2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d42c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d42c2-107">Правила доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="d42c2-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="d42c2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d42c2-108">Properties</span></span>
|<span data-ttu-id="d42c2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d42c2-109">Property</span></span>|<span data-ttu-id="d42c2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d42c2-110">Type</span></span>|<span data-ttu-id="d42c2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d42c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d42c2-112">девицекласс</span><span class="sxs-lookup"><span data-stu-id="d42c2-112">deviceClass</span></span>|[<span data-ttu-id="d42c2-113">девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="d42c2-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="d42c2-114">Класс устройства, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="d42c2-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="d42c2-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="d42c2-115">accessLevel</span></span>|[<span data-ttu-id="d42c2-116">девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="d42c2-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="d42c2-117">Уровень доступа для Exchange, предоставляемый этим правилом.</span><span class="sxs-lookup"><span data-stu-id="d42c2-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="d42c2-118">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="d42c2-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d42c2-119">Связи</span><span class="sxs-lookup"><span data-stu-id="d42c2-119">Relationships</span></span>
<span data-ttu-id="d42c2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d42c2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d42c2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d42c2-121">JSON Representation</span></span>
<span data-ttu-id="d42c2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d42c2-122">Here is a JSON representation of the resource.</span></span>
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




