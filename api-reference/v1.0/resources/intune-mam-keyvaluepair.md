---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6a2365223904f61b6c0b4aada6a26cf5888acf0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445831"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="7b44a-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="7b44a-103">keyValuePair resource type</span></span>

<span data-ttu-id="7b44a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b44a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b44a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b44a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b44a-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="7b44a-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="7b44a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b44a-107">Properties</span></span>
|<span data-ttu-id="7b44a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b44a-108">Property</span></span>|<span data-ttu-id="7b44a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b44a-109">Type</span></span>|<span data-ttu-id="7b44a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b44a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b44a-111">name</span><span class="sxs-lookup"><span data-stu-id="7b44a-111">name</span></span>|<span data-ttu-id="7b44a-112">String</span><span class="sxs-lookup"><span data-stu-id="7b44a-112">String</span></span>|<span data-ttu-id="7b44a-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="7b44a-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="7b44a-114">value</span><span class="sxs-lookup"><span data-stu-id="7b44a-114">value</span></span>|<span data-ttu-id="7b44a-115">String</span><span class="sxs-lookup"><span data-stu-id="7b44a-115">String</span></span>|<span data-ttu-id="7b44a-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="7b44a-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b44a-117">Связи</span><span class="sxs-lookup"><span data-stu-id="7b44a-117">Relationships</span></span>
<span data-ttu-id="7b44a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7b44a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b44a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b44a-119">JSON Representation</span></span>
<span data-ttu-id="7b44a-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b44a-120">Here is a JSON representation of the resource.</span></span>
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







