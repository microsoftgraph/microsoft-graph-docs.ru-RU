---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0d112c76e03f45ba7bf28fea3b6d219745c4332
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283221"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="4965a-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="4965a-103">keyValue resource type</span></span>

<span data-ttu-id="4965a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4965a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4965a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4965a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4965a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4965a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4965a-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="4965a-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="4965a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4965a-108">Properties</span></span>
|<span data-ttu-id="4965a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4965a-109">Property</span></span>|<span data-ttu-id="4965a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4965a-110">Type</span></span>|<span data-ttu-id="4965a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4965a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4965a-112">key</span><span class="sxs-lookup"><span data-stu-id="4965a-112">key</span></span>|<span data-ttu-id="4965a-113">String</span><span class="sxs-lookup"><span data-stu-id="4965a-113">String</span></span>|<span data-ttu-id="4965a-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="4965a-114">Key.</span></span>|
|<span data-ttu-id="4965a-115">value</span><span class="sxs-lookup"><span data-stu-id="4965a-115">value</span></span>|<span data-ttu-id="4965a-116">String</span><span class="sxs-lookup"><span data-stu-id="4965a-116">String</span></span>|<span data-ttu-id="4965a-117">Значение</span><span class="sxs-lookup"><span data-stu-id="4965a-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4965a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="4965a-118">Relationships</span></span>
<span data-ttu-id="4965a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="4965a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4965a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4965a-120">JSON Representation</span></span>
<span data-ttu-id="4965a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4965a-121">Here is a JSON representation of the resource.</span></span>
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




