---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 657df623da3498588d9d6aa6f6d6fb121285c33e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529769"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="cfc5e-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="cfc5e-103">keyValue resource type</span></span>

<span data-ttu-id="cfc5e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cfc5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfc5e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfc5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfc5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfc5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfc5e-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="cfc5e-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="cfc5e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfc5e-108">Properties</span></span>
|<span data-ttu-id="cfc5e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfc5e-109">Property</span></span>|<span data-ttu-id="cfc5e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cfc5e-110">Type</span></span>|<span data-ttu-id="cfc5e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cfc5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfc5e-112">ключа</span><span class="sxs-lookup"><span data-stu-id="cfc5e-112">key</span></span>|<span data-ttu-id="cfc5e-113">String</span><span class="sxs-lookup"><span data-stu-id="cfc5e-113">String</span></span>|<span data-ttu-id="cfc5e-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="cfc5e-114">Key.</span></span>|
|<span data-ttu-id="cfc5e-115">value</span><span class="sxs-lookup"><span data-stu-id="cfc5e-115">value</span></span>|<span data-ttu-id="cfc5e-116">String</span><span class="sxs-lookup"><span data-stu-id="cfc5e-116">String</span></span>|<span data-ttu-id="cfc5e-117">Значение</span><span class="sxs-lookup"><span data-stu-id="cfc5e-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfc5e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="cfc5e-118">Relationships</span></span>
<span data-ttu-id="cfc5e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="cfc5e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfc5e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfc5e-120">JSON Representation</span></span>
<span data-ttu-id="cfc5e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfc5e-121">Here is a JSON representation of the resource.</span></span>
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



