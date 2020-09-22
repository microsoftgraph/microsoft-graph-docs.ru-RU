---
title: Тип ресурса Деливерйоптимизатионграупидкустом
description: Тип идентификатора настраиваемой группы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 558dbf0b0e1d2b927da8c4d7e7f159d31b4e4f95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078376"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="c08cf-103">Тип ресурса Деливерйоптимизатионграупидкустом</span><span class="sxs-lookup"><span data-stu-id="c08cf-103">deliveryOptimizationGroupIdCustom resource type</span></span>

<span data-ttu-id="c08cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c08cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c08cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c08cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c08cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c08cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c08cf-107">Тип идентификатора настраиваемой группы</span><span class="sxs-lookup"><span data-stu-id="c08cf-107">Custom group id type</span></span>


<span data-ttu-id="c08cf-108">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="c08cf-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c08cf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c08cf-109">Properties</span></span>
|<span data-ttu-id="c08cf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c08cf-110">Property</span></span>|<span data-ttu-id="c08cf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c08cf-111">Type</span></span>|<span data-ttu-id="c08cf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c08cf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c08cf-113">граупидкустом</span><span class="sxs-lookup"><span data-stu-id="c08cf-113">groupIdCustom</span></span>|<span data-ttu-id="c08cf-114">String</span><span class="sxs-lookup"><span data-stu-id="c08cf-114">String</span></span>|<span data-ttu-id="c08cf-115">Указывает произвольный идентификатор группы, к которому относится устройство.</span><span class="sxs-lookup"><span data-stu-id="c08cf-115">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="c08cf-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="c08cf-116">Relationships</span></span>
<span data-ttu-id="c08cf-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c08cf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c08cf-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c08cf-118">JSON Representation</span></span>
<span data-ttu-id="c08cf-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c08cf-119">Here is a JSON representation of the resource.</span></span>
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






