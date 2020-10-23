---
title: Тип ресурса Девицекомплианцеполицискрипт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1a87354782ff1e8b4d90eb3c6eb5c69e1332fd4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731425"
---
# <a name="devicecompliancepolicyscript-resource-type"></a><span data-ttu-id="c354b-103">Тип ресурса Девицекомплианцеполицискрипт</span><span class="sxs-lookup"><span data-stu-id="c354b-103">deviceCompliancePolicyScript resource type</span></span>

<span data-ttu-id="c354b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c354b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c354b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c354b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c354b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c354b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c354b-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c354b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c354b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c354b-108">Properties</span></span>
|<span data-ttu-id="c354b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c354b-109">Property</span></span>|<span data-ttu-id="c354b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c354b-110">Type</span></span>|<span data-ttu-id="c354b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c354b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c354b-112">девицекомплианцескриптид</span><span class="sxs-lookup"><span data-stu-id="c354b-112">deviceComplianceScriptId</span></span>|<span data-ttu-id="c354b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c354b-113">String</span></span>|<span data-ttu-id="c354b-114">Идентификатор сценария соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="c354b-114">Device compliance script Id.</span></span>|
|<span data-ttu-id="c354b-115">рулесконтент</span><span class="sxs-lookup"><span data-stu-id="c354b-115">rulesContent</span></span>|<span data-ttu-id="c354b-116">Binary</span><span class="sxs-lookup"><span data-stu-id="c354b-116">Binary</span></span>|<span data-ttu-id="c354b-117">JSON правил.</span><span class="sxs-lookup"><span data-stu-id="c354b-117">Json of the rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c354b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c354b-118">Relationships</span></span>
<span data-ttu-id="c354b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c354b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c354b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c354b-120">JSON Representation</span></span>
<span data-ttu-id="c354b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c354b-121">Here is a JSON representation of the resource.</span></span>
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





