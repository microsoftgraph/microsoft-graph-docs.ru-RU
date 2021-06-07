---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3deb1d366396bf97133b4984bda2b67609fcdee6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751666"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="319a2-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="319a2-103">keyValuePair resource type</span></span>

<span data-ttu-id="319a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="319a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="319a2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="319a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="319a2-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="319a2-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="319a2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="319a2-107">Properties</span></span>
|<span data-ttu-id="319a2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="319a2-108">Property</span></span>|<span data-ttu-id="319a2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="319a2-109">Type</span></span>|<span data-ttu-id="319a2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="319a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="319a2-111">name</span><span class="sxs-lookup"><span data-stu-id="319a2-111">name</span></span>|<span data-ttu-id="319a2-112">String</span><span class="sxs-lookup"><span data-stu-id="319a2-112">String</span></span>|<span data-ttu-id="319a2-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="319a2-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="319a2-114">value</span><span class="sxs-lookup"><span data-stu-id="319a2-114">value</span></span>|<span data-ttu-id="319a2-115">String</span><span class="sxs-lookup"><span data-stu-id="319a2-115">String</span></span>|<span data-ttu-id="319a2-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="319a2-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="319a2-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="319a2-117">Relationships</span></span>
<span data-ttu-id="319a2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="319a2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="319a2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="319a2-119">JSON Representation</span></span>
<span data-ttu-id="319a2-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="319a2-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```




