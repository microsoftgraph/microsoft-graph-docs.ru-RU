---
title: Тип ресурса МакосассоЦиатеддомаинскэйвалуепаир
description: Комбинация "ключ — значение" для связанных доменов
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08a59f0566da2e2dffa64c059cc913923ec5cf58
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790323"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a><span data-ttu-id="3d975-103">Тип ресурса МакосассоЦиатеддомаинскэйвалуепаир</span><span class="sxs-lookup"><span data-stu-id="3d975-103">macOSAssociatedDomainsKeyValuePair resource type</span></span>

> <span data-ttu-id="3d975-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d975-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d975-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d975-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d975-106">Комбинация "ключ — значение" для связанных доменов</span><span class="sxs-lookup"><span data-stu-id="3d975-106">Key value pair for associated domains</span></span>


<span data-ttu-id="3d975-107">Наследуется от [KeyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3d975-107">Inherits from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3d975-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d975-108">Properties</span></span>
|<span data-ttu-id="3d975-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d975-109">Property</span></span>|<span data-ttu-id="3d975-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3d975-110">Type</span></span>|<span data-ttu-id="3d975-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3d975-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d975-112">name</span><span class="sxs-lookup"><span data-stu-id="3d975-112">name</span></span>|<span data-ttu-id="3d975-113">String</span><span class="sxs-lookup"><span data-stu-id="3d975-113">String</span></span>|<span data-ttu-id="3d975-114">Имя для этой ключевой [РазkeyValuePairа](../resources/intune-shared-keyvaluepair.md) , унаследованной от</span><span class="sxs-lookup"><span data-stu-id="3d975-114">Name for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|
|<span data-ttu-id="3d975-115">value</span><span class="sxs-lookup"><span data-stu-id="3d975-115">value</span></span>|<span data-ttu-id="3d975-116">String</span><span class="sxs-lookup"><span data-stu-id="3d975-116">String</span></span>|<span data-ttu-id="3d975-117">Значение для этой заданной для этой основе ключа, унаследованной от [KeyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3d975-117">Value for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d975-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3d975-118">Relationships</span></span>
<span data-ttu-id="3d975-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3d975-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d975-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d975-120">JSON Representation</span></span>
<span data-ttu-id="3d975-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d975-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsKeyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsKeyValuePair",
  "name": "String",
  "value": "String"
}
```



