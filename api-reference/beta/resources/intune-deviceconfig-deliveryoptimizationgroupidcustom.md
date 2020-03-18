---
title: Тип ресурса Деливерйоптимизатионграупидкустом
description: Тип идентификатора настраиваемой группы
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e3dd542a99a7eace79fbc3318117dbf7c539ee79
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794370"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="84632-103">Тип ресурса Деливерйоптимизатионграупидкустом</span><span class="sxs-lookup"><span data-stu-id="84632-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="84632-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84632-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84632-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84632-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84632-106">Тип идентификатора настраиваемой группы</span><span class="sxs-lookup"><span data-stu-id="84632-106">Custom group id type</span></span>


<span data-ttu-id="84632-107">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="84632-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84632-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="84632-108">Properties</span></span>
|<span data-ttu-id="84632-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="84632-109">Property</span></span>|<span data-ttu-id="84632-110">Тип</span><span class="sxs-lookup"><span data-stu-id="84632-110">Type</span></span>|<span data-ttu-id="84632-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84632-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84632-112">граупидкустом</span><span class="sxs-lookup"><span data-stu-id="84632-112">groupIdCustom</span></span>|<span data-ttu-id="84632-113">String</span><span class="sxs-lookup"><span data-stu-id="84632-113">String</span></span>|<span data-ttu-id="84632-114">Указывает произвольный идентификатор группы, к которому относится устройство.</span><span class="sxs-lookup"><span data-stu-id="84632-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="84632-115">Связи</span><span class="sxs-lookup"><span data-stu-id="84632-115">Relationships</span></span>
<span data-ttu-id="84632-116">Нет</span><span class="sxs-lookup"><span data-stu-id="84632-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84632-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84632-117">JSON Representation</span></span>
<span data-ttu-id="84632-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84632-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```



