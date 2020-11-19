---
title: Тип ресурса Девицекомплианцеполицискрипт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1299848a53ea924278af06a71db9f1554849b53
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216166"
---
# <a name="devicecompliancepolicyscript-resource-type"></a><span data-ttu-id="08b7d-103">Тип ресурса Девицекомплианцеполицискрипт</span><span class="sxs-lookup"><span data-stu-id="08b7d-103">deviceCompliancePolicyScript resource type</span></span>

<span data-ttu-id="08b7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08b7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08b7d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08b7d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08b7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08b7d-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="08b7d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="08b7d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="08b7d-108">Properties</span></span>
|<span data-ttu-id="08b7d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="08b7d-109">Property</span></span>|<span data-ttu-id="08b7d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="08b7d-110">Type</span></span>|<span data-ttu-id="08b7d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="08b7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08b7d-112">девицекомплианцескриптид</span><span class="sxs-lookup"><span data-stu-id="08b7d-112">deviceComplianceScriptId</span></span>|<span data-ttu-id="08b7d-113">String</span><span class="sxs-lookup"><span data-stu-id="08b7d-113">String</span></span>|<span data-ttu-id="08b7d-114">Идентификатор сценария соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="08b7d-114">Device compliance script Id.</span></span>|
|<span data-ttu-id="08b7d-115">рулесконтент</span><span class="sxs-lookup"><span data-stu-id="08b7d-115">rulesContent</span></span>|<span data-ttu-id="08b7d-116">Binary</span><span class="sxs-lookup"><span data-stu-id="08b7d-116">Binary</span></span>|<span data-ttu-id="08b7d-117">JSON правил.</span><span class="sxs-lookup"><span data-stu-id="08b7d-117">Json of the rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08b7d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="08b7d-118">Relationships</span></span>
<span data-ttu-id="08b7d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="08b7d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08b7d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08b7d-120">JSON Representation</span></span>
<span data-ttu-id="08b7d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08b7d-121">Here is a JSON representation of the resource.</span></span>
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




