---
title: Тип ресурса Деливерйоптимизатионграупидкустом
description: Тип идентификатора настраиваемой группы
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2e0fa587c312d4e4eef43873f08842ac5c7c79b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333403"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="32499-103">Тип ресурса Деливерйоптимизатионграупидкустом</span><span class="sxs-lookup"><span data-stu-id="32499-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="32499-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32499-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32499-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32499-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32499-106">Тип идентификатора настраиваемой группы</span><span class="sxs-lookup"><span data-stu-id="32499-106">Custom group id type</span></span>


<span data-ttu-id="32499-107">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="32499-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32499-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="32499-108">Properties</span></span>
|<span data-ttu-id="32499-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="32499-109">Property</span></span>|<span data-ttu-id="32499-110">Тип</span><span class="sxs-lookup"><span data-stu-id="32499-110">Type</span></span>|<span data-ttu-id="32499-111">Описание</span><span class="sxs-lookup"><span data-stu-id="32499-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32499-112">граупидкустом</span><span class="sxs-lookup"><span data-stu-id="32499-112">groupIdCustom</span></span>|<span data-ttu-id="32499-113">String</span><span class="sxs-lookup"><span data-stu-id="32499-113">String</span></span>|<span data-ttu-id="32499-114">Указывает произвольный идентификатор группы, к которому относится устройство.</span><span class="sxs-lookup"><span data-stu-id="32499-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="32499-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="32499-115">Relationships</span></span>
<span data-ttu-id="32499-116">Нет</span><span class="sxs-lookup"><span data-stu-id="32499-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32499-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32499-117">JSON Representation</span></span>
<span data-ttu-id="32499-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32499-118">Here is a JSON representation of the resource.</span></span>
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



