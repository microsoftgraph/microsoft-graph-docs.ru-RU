---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 317736fd016ca457a7fad9536ce71f00b6954b3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460508"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="b433e-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="b433e-103">keyValue resource type</span></span>

> <span data-ttu-id="b433e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b433e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b433e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b433e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b433e-106">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="b433e-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b433e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b433e-107">Properties</span></span>
|<span data-ttu-id="b433e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b433e-108">Property</span></span>|<span data-ttu-id="b433e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b433e-109">Type</span></span>|<span data-ttu-id="b433e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b433e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b433e-111">ключа</span><span class="sxs-lookup"><span data-stu-id="b433e-111">key</span></span>|<span data-ttu-id="b433e-112">String</span><span class="sxs-lookup"><span data-stu-id="b433e-112">String</span></span>|<span data-ttu-id="b433e-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="b433e-113">Key.</span></span>|
|<span data-ttu-id="b433e-114">value</span><span class="sxs-lookup"><span data-stu-id="b433e-114">value</span></span>|<span data-ttu-id="b433e-115">String</span><span class="sxs-lookup"><span data-stu-id="b433e-115">String</span></span>|<span data-ttu-id="b433e-116">Значение</span><span class="sxs-lookup"><span data-stu-id="b433e-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b433e-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="b433e-117">Relationships</span></span>
<span data-ttu-id="b433e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b433e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b433e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b433e-119">JSON Representation</span></span>
<span data-ttu-id="b433e-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b433e-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





