---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0ced5c90f0e36906a534523836e7be3b99eb797
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533192"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="c861a-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="c861a-103">keyValuePair resource type</span></span>

<span data-ttu-id="c861a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c861a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c861a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c861a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c861a-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="c861a-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="c861a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c861a-107">Properties</span></span>
|<span data-ttu-id="c861a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c861a-108">Property</span></span>|<span data-ttu-id="c861a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c861a-109">Type</span></span>|<span data-ttu-id="c861a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c861a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c861a-111">name</span><span class="sxs-lookup"><span data-stu-id="c861a-111">name</span></span>|<span data-ttu-id="c861a-112">String</span><span class="sxs-lookup"><span data-stu-id="c861a-112">String</span></span>|<span data-ttu-id="c861a-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="c861a-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="c861a-114">value</span><span class="sxs-lookup"><span data-stu-id="c861a-114">value</span></span>|<span data-ttu-id="c861a-115">String</span><span class="sxs-lookup"><span data-stu-id="c861a-115">String</span></span>|<span data-ttu-id="c861a-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="c861a-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="c861a-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c861a-117">Relationships</span></span>
<span data-ttu-id="c861a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c861a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c861a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c861a-119">JSON Representation</span></span>
<span data-ttu-id="c861a-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c861a-120">Here is a JSON representation of the resource.</span></span>
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




