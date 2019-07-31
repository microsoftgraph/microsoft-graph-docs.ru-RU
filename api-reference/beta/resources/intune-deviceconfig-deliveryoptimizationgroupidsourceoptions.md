---
title: Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс
description: Тип параметров идентификатора группы
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fc2c900828526ac4d2788c2b91e669bae04f452f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970747"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="3cb09-103">Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс</span><span class="sxs-lookup"><span data-stu-id="3cb09-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="3cb09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cb09-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3cb09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cb09-106">Тип параметров идентификатора группы</span><span class="sxs-lookup"><span data-stu-id="3cb09-106">Group id options type</span></span>


<span data-ttu-id="3cb09-107">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="3cb09-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3cb09-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cb09-108">Properties</span></span>
|<span data-ttu-id="3cb09-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3cb09-109">Property</span></span>|<span data-ttu-id="3cb09-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb09-110">Type</span></span>|<span data-ttu-id="3cb09-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cb09-112">Граупидсаурцеоптион</span><span class="sxs-lookup"><span data-stu-id="3cb09-112">groupIdSourceOption</span></span>|[<span data-ttu-id="3cb09-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="3cb09-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="3cb09-114">Установите эту политику, чтобы ограничить выбор однорангового узла определенным источником.</span><span class="sxs-lookup"><span data-stu-id="3cb09-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="3cb09-115">Возможные значения: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="3cb09-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cb09-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="3cb09-116">Relationships</span></span>
<span data-ttu-id="3cb09-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3cb09-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3cb09-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3cb09-118">JSON Representation</span></span>
<span data-ttu-id="3cb09-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cb09-119">Here is a JSON representation of the resource.</span></span>
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





