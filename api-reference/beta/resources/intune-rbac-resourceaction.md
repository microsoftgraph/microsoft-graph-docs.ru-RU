---
title: Тип ресурса resourceAction
description: Набор разрешенных и запрещенных действий для ресурса.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 837371f89d144026d97d1e122711a26784800b75
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527552"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="97d1f-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="97d1f-103">resourceAction resource type</span></span>

<span data-ttu-id="97d1f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="97d1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97d1f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97d1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97d1f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97d1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d1f-107">Набор разрешенных и запрещенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="97d1f-107">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="97d1f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="97d1f-108">Properties</span></span>
|<span data-ttu-id="97d1f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="97d1f-109">Property</span></span>|<span data-ttu-id="97d1f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="97d1f-110">Type</span></span>|<span data-ttu-id="97d1f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="97d1f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d1f-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="97d1f-112">allowedResourceActions</span></span>|<span data-ttu-id="97d1f-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="97d1f-113">String collection</span></span>|<span data-ttu-id="97d1f-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="97d1f-114">Allowed Actions</span></span>|
|<span data-ttu-id="97d1f-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="97d1f-115">notAllowedResourceActions</span></span>|<span data-ttu-id="97d1f-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="97d1f-116">String collection</span></span>|<span data-ttu-id="97d1f-117">Действия не разрешены.</span><span class="sxs-lookup"><span data-stu-id="97d1f-117">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97d1f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="97d1f-118">Relationships</span></span>
<span data-ttu-id="97d1f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="97d1f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97d1f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97d1f-120">JSON Representation</span></span>
<span data-ttu-id="97d1f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97d1f-121">Here is a JSON representation of the resource.</span></span>
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



