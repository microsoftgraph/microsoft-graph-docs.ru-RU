---
title: Тип ресурса Девицекомплианцеполицискрипт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a56c650aa5f7341b49a8cda79bd833fecffb2a65
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979401"
---
# <a name="devicecompliancepolicyscript-resource-type"></a><span data-ttu-id="c01ad-103">Тип ресурса Девицекомплианцеполицискрипт</span><span class="sxs-lookup"><span data-stu-id="c01ad-103">deviceCompliancePolicyScript resource type</span></span>

<span data-ttu-id="c01ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c01ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c01ad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c01ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c01ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c01ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c01ad-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c01ad-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c01ad-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c01ad-108">Properties</span></span>
|<span data-ttu-id="c01ad-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c01ad-109">Property</span></span>|<span data-ttu-id="c01ad-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c01ad-110">Type</span></span>|<span data-ttu-id="c01ad-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c01ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c01ad-112">девицекомплианцескриптид</span><span class="sxs-lookup"><span data-stu-id="c01ad-112">deviceComplianceScriptId</span></span>|<span data-ttu-id="c01ad-113">String</span><span class="sxs-lookup"><span data-stu-id="c01ad-113">String</span></span>|<span data-ttu-id="c01ad-114">Идентификатор сценария соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="c01ad-114">Device compliance script Id.</span></span>|
|<span data-ttu-id="c01ad-115">рулесконтент</span><span class="sxs-lookup"><span data-stu-id="c01ad-115">rulesContent</span></span>|<span data-ttu-id="c01ad-116">Binary</span><span class="sxs-lookup"><span data-stu-id="c01ad-116">Binary</span></span>|<span data-ttu-id="c01ad-117">JSON правил.</span><span class="sxs-lookup"><span data-stu-id="c01ad-117">Json of the rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c01ad-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c01ad-118">Relationships</span></span>
<span data-ttu-id="c01ad-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c01ad-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c01ad-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c01ad-120">JSON Representation</span></span>
<span data-ttu-id="c01ad-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c01ad-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyScript",
  "deviceComplianceScriptId": "String",
  "rulesContent": "binary"
}
```






