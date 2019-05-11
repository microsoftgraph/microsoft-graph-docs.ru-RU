---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc34bad30ff5bc33f60e6ec4e561e6644b97cc37
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938662"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="47df1-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="47df1-103">keyValuePair resource type</span></span>

> <span data-ttu-id="47df1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47df1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47df1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47df1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47df1-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="47df1-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="47df1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="47df1-107">Properties</span></span>
|<span data-ttu-id="47df1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="47df1-108">Property</span></span>|<span data-ttu-id="47df1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="47df1-109">Type</span></span>|<span data-ttu-id="47df1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="47df1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47df1-111">name</span><span class="sxs-lookup"><span data-stu-id="47df1-111">name</span></span>|<span data-ttu-id="47df1-112">String</span><span class="sxs-lookup"><span data-stu-id="47df1-112">String</span></span>|<span data-ttu-id="47df1-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="47df1-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="47df1-114">value</span><span class="sxs-lookup"><span data-stu-id="47df1-114">value</span></span>|<span data-ttu-id="47df1-115">String</span><span class="sxs-lookup"><span data-stu-id="47df1-115">String</span></span>|<span data-ttu-id="47df1-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="47df1-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="47df1-117">Связи</span><span class="sxs-lookup"><span data-stu-id="47df1-117">Relationships</span></span>
<span data-ttu-id="47df1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="47df1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47df1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47df1-119">JSON Representation</span></span>
<span data-ttu-id="47df1-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47df1-120">Here is a JSON representation of the resource.</span></span>
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




