---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b86c1cbfcee4519d93bdfa704bc5d283343342c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255828"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="2f272-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="2f272-103">keyValuePair resource type</span></span>

<span data-ttu-id="2f272-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f272-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f272-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f272-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f272-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f272-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f272-107">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="2f272-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="2f272-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f272-108">Properties</span></span>
|<span data-ttu-id="2f272-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f272-109">Property</span></span>|<span data-ttu-id="2f272-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2f272-110">Type</span></span>|<span data-ttu-id="2f272-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2f272-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f272-112">name</span><span class="sxs-lookup"><span data-stu-id="2f272-112">name</span></span>|<span data-ttu-id="2f272-113">String</span><span class="sxs-lookup"><span data-stu-id="2f272-113">String</span></span>|<span data-ttu-id="2f272-114">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="2f272-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="2f272-115">value</span><span class="sxs-lookup"><span data-stu-id="2f272-115">value</span></span>|<span data-ttu-id="2f272-116">String</span><span class="sxs-lookup"><span data-stu-id="2f272-116">String</span></span>|<span data-ttu-id="2f272-117">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="2f272-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f272-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2f272-118">Relationships</span></span>
<span data-ttu-id="2f272-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2f272-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f272-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f272-120">JSON Representation</span></span>
<span data-ttu-id="2f272-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f272-121">Here is a JSON representation of the resource.</span></span>
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




