---
title: Тип ресурса Деливерйоптимизатионграупидкустом
description: Тип идентификатора настраиваемой группы
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3b00920d0ead3df5fe694e110825615f449ef4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177975"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="bcfe7-103">Тип ресурса Деливерйоптимизатионграупидкустом</span><span class="sxs-lookup"><span data-stu-id="bcfe7-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="bcfe7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcfe7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcfe7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcfe7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcfe7-106">Тип идентификатора настраиваемой группы</span><span class="sxs-lookup"><span data-stu-id="bcfe7-106">Custom group id type</span></span>


<span data-ttu-id="bcfe7-107">НаСледуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="bcfe7-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bcfe7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bcfe7-108">Properties</span></span>
|<span data-ttu-id="bcfe7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcfe7-109">Property</span></span>|<span data-ttu-id="bcfe7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bcfe7-110">Type</span></span>|<span data-ttu-id="bcfe7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bcfe7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcfe7-112">Граупидкустом</span><span class="sxs-lookup"><span data-stu-id="bcfe7-112">groupIdCustom</span></span>|<span data-ttu-id="bcfe7-113">String</span><span class="sxs-lookup"><span data-stu-id="bcfe7-113">String</span></span>|<span data-ttu-id="bcfe7-114">Указывает произвольный идентификатор группы, к которому относится устройство.</span><span class="sxs-lookup"><span data-stu-id="bcfe7-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcfe7-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="bcfe7-115">Relationships</span></span>
<span data-ttu-id="bcfe7-116">Нет</span><span class="sxs-lookup"><span data-stu-id="bcfe7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bcfe7-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bcfe7-117">JSON Representation</span></span>
<span data-ttu-id="bcfe7-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcfe7-118">Here is a JSON representation of the resource.</span></span>
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




