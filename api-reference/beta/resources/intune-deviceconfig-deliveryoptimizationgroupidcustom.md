---
title: Тип ресурса Деливерйоптимизатионграупидкустом
description: Тип идентификатора настраиваемой группы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3565ff8e0e13c3a0964882c159e0fa156aa43c7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696218"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="7701e-103">Тип ресурса Деливерйоптимизатионграупидкустом</span><span class="sxs-lookup"><span data-stu-id="7701e-103">deliveryOptimizationGroupIdCustom resource type</span></span>

<span data-ttu-id="7701e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7701e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7701e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7701e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7701e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7701e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7701e-107">Тип идентификатора настраиваемой группы</span><span class="sxs-lookup"><span data-stu-id="7701e-107">Custom group id type</span></span>


<span data-ttu-id="7701e-108">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="7701e-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7701e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7701e-109">Properties</span></span>
|<span data-ttu-id="7701e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7701e-110">Property</span></span>|<span data-ttu-id="7701e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7701e-111">Type</span></span>|<span data-ttu-id="7701e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7701e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7701e-113">граупидкустом</span><span class="sxs-lookup"><span data-stu-id="7701e-113">groupIdCustom</span></span>|<span data-ttu-id="7701e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="7701e-114">String</span></span>|<span data-ttu-id="7701e-115">Указывает произвольный идентификатор группы, к которому относится устройство.</span><span class="sxs-lookup"><span data-stu-id="7701e-115">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="7701e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="7701e-116">Relationships</span></span>
<span data-ttu-id="7701e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="7701e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7701e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7701e-118">JSON Representation</span></span>
<span data-ttu-id="7701e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7701e-119">Here is a JSON representation of the resource.</span></span>
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





