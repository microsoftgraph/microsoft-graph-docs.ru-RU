---
title: Тип ресурса Деливерйоптимизатионграупидкустом
description: Тип идентификатора настраиваемой группы
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0b818a8c9e2a6a3cb13a8caa00b2115cf7f52b3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420481"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="9c7ab-103">Тип ресурса Деливерйоптимизатионграупидкустом</span><span class="sxs-lookup"><span data-stu-id="9c7ab-103">deliveryOptimizationGroupIdCustom resource type</span></span>

<span data-ttu-id="9c7ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c7ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c7ab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c7ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c7ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c7ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c7ab-107">Тип идентификатора настраиваемой группы</span><span class="sxs-lookup"><span data-stu-id="9c7ab-107">Custom group id type</span></span>


<span data-ttu-id="9c7ab-108">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="9c7ab-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9c7ab-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c7ab-109">Properties</span></span>
|<span data-ttu-id="9c7ab-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c7ab-110">Property</span></span>|<span data-ttu-id="9c7ab-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9c7ab-111">Type</span></span>|<span data-ttu-id="9c7ab-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9c7ab-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c7ab-113">граупидкустом</span><span class="sxs-lookup"><span data-stu-id="9c7ab-113">groupIdCustom</span></span>|<span data-ttu-id="9c7ab-114">String</span><span class="sxs-lookup"><span data-stu-id="9c7ab-114">String</span></span>|<span data-ttu-id="9c7ab-115">Указывает произвольный идентификатор группы, к которому относится устройство.</span><span class="sxs-lookup"><span data-stu-id="9c7ab-115">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c7ab-116">Связи</span><span class="sxs-lookup"><span data-stu-id="9c7ab-116">Relationships</span></span>
<span data-ttu-id="9c7ab-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9c7ab-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c7ab-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c7ab-118">JSON Representation</span></span>
<span data-ttu-id="9c7ab-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c7ab-119">Here is a JSON representation of the resource.</span></span>
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



