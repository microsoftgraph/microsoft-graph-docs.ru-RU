---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb3e5e47b6c4594fa366101e83cc1453400db00c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984392"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="6fb9c-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="6fb9c-103">keyValuePair resource type</span></span>

<span data-ttu-id="6fb9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fb9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fb9c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fb9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fb9c-106">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="6fb9c-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="6fb9c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fb9c-107">Properties</span></span>
|<span data-ttu-id="6fb9c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fb9c-108">Property</span></span>|<span data-ttu-id="6fb9c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6fb9c-109">Type</span></span>|<span data-ttu-id="6fb9c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6fb9c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb9c-111">name</span><span class="sxs-lookup"><span data-stu-id="6fb9c-111">name</span></span>|<span data-ttu-id="6fb9c-112">String</span><span class="sxs-lookup"><span data-stu-id="6fb9c-112">String</span></span>|<span data-ttu-id="6fb9c-113">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="6fb9c-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="6fb9c-114">value</span><span class="sxs-lookup"><span data-stu-id="6fb9c-114">value</span></span>|<span data-ttu-id="6fb9c-115">String</span><span class="sxs-lookup"><span data-stu-id="6fb9c-115">String</span></span>|<span data-ttu-id="6fb9c-116">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="6fb9c-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fb9c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="6fb9c-117">Relationships</span></span>
<span data-ttu-id="6fb9c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6fb9c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fb9c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fb9c-119">JSON Representation</span></span>
<span data-ttu-id="6fb9c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fb9c-120">Here is a JSON representation of the resource.</span></span>
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









