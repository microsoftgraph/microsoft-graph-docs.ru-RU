---
title: Тип ресурса resourceAction
description: Набор разрешенных и не разрешенных действий для ресурса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3517a4608691b65ce33ac40b4a9d9929bd277f31
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752436"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="7a80e-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="7a80e-103">resourceAction resource type</span></span>

<span data-ttu-id="7a80e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a80e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a80e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a80e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a80e-106">Набор разрешенных и не разрешенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="7a80e-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="7a80e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a80e-107">Properties</span></span>
|<span data-ttu-id="7a80e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a80e-108">Property</span></span>|<span data-ttu-id="7a80e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7a80e-109">Type</span></span>|<span data-ttu-id="7a80e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a80e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a80e-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="7a80e-111">allowedResourceActions</span></span>|<span data-ttu-id="7a80e-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7a80e-112">String collection</span></span>|<span data-ttu-id="7a80e-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="7a80e-113">Allowed Actions</span></span>|
|<span data-ttu-id="7a80e-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="7a80e-114">notAllowedResourceActions</span></span>|<span data-ttu-id="7a80e-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7a80e-115">String collection</span></span>|<span data-ttu-id="7a80e-116">Не разрешенные действия.</span><span class="sxs-lookup"><span data-stu-id="7a80e-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a80e-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="7a80e-117">Relationships</span></span>
<span data-ttu-id="7a80e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7a80e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a80e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a80e-119">JSON Representation</span></span>
<span data-ttu-id="7a80e-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a80e-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




