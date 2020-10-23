---
title: Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс
description: Тип параметров идентификатора группы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1dc2c2ac96ffdbd166c940400740de03578b5ff1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735871"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="c7c92-103">Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс</span><span class="sxs-lookup"><span data-stu-id="c7c92-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

<span data-ttu-id="c7c92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7c92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7c92-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7c92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7c92-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7c92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c92-107">Тип параметров идентификатора группы</span><span class="sxs-lookup"><span data-stu-id="c7c92-107">Group id options type</span></span>


<span data-ttu-id="c7c92-108">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="c7c92-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7c92-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7c92-109">Properties</span></span>
|<span data-ttu-id="c7c92-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7c92-110">Property</span></span>|<span data-ttu-id="c7c92-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c7c92-111">Type</span></span>|<span data-ttu-id="c7c92-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c7c92-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c92-113">граупидсаурцеоптион</span><span class="sxs-lookup"><span data-stu-id="c7c92-113">groupIdSourceOption</span></span>|[<span data-ttu-id="c7c92-114">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="c7c92-114">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="c7c92-115">Установите эту политику, чтобы ограничить выбор однорангового узла определенным источником.</span><span class="sxs-lookup"><span data-stu-id="c7c92-115">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="c7c92-116">Возможные значения: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="c7c92-116">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7c92-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c7c92-117">Relationships</span></span>
<span data-ttu-id="c7c92-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c7c92-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7c92-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7c92-119">JSON Representation</span></span>
<span data-ttu-id="c7c92-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7c92-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```





