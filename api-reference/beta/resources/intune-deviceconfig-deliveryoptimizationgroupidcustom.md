---
title: Тип ресурса Деливерйоптимизатионграупидкустом
description: Тип идентификатора настраиваемой группы
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e439b9d4777a0b0c513d750d0b5e35783dbd9a1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947255"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="ee379-103">Тип ресурса Деливерйоптимизатионграупидкустом</span><span class="sxs-lookup"><span data-stu-id="ee379-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="ee379-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee379-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee379-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee379-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee379-106">Тип идентификатора настраиваемой группы</span><span class="sxs-lookup"><span data-stu-id="ee379-106">Custom group id type</span></span>


<span data-ttu-id="ee379-107">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="ee379-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee379-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee379-108">Properties</span></span>
|<span data-ttu-id="ee379-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee379-109">Property</span></span>|<span data-ttu-id="ee379-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ee379-110">Type</span></span>|<span data-ttu-id="ee379-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ee379-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee379-112">Граупидкустом</span><span class="sxs-lookup"><span data-stu-id="ee379-112">groupIdCustom</span></span>|<span data-ttu-id="ee379-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ee379-113">String</span></span>|<span data-ttu-id="ee379-114">Указывает произвольный идентификатор группы, к которому относится устройство.</span><span class="sxs-lookup"><span data-stu-id="ee379-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee379-115">Связи</span><span class="sxs-lookup"><span data-stu-id="ee379-115">Relationships</span></span>
<span data-ttu-id="ee379-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ee379-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee379-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee379-117">JSON Representation</span></span>
<span data-ttu-id="ee379-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee379-118">Here is a JSON representation of the resource.</span></span>
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




