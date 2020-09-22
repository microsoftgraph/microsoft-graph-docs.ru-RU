---
title: Тип ресурса resourceAction
description: Набор разрешенных и запрещенных действий для ресурса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c7b38b3b534465145e30076c175d9da96f25b062
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095228"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="64214-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="64214-103">resourceAction resource type</span></span>

<span data-ttu-id="64214-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64214-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64214-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64214-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64214-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64214-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64214-107">Набор разрешенных и запрещенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="64214-107">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="64214-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="64214-108">Properties</span></span>
|<span data-ttu-id="64214-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="64214-109">Property</span></span>|<span data-ttu-id="64214-110">Тип</span><span class="sxs-lookup"><span data-stu-id="64214-110">Type</span></span>|<span data-ttu-id="64214-111">Описание</span><span class="sxs-lookup"><span data-stu-id="64214-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64214-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="64214-112">allowedResourceActions</span></span>|<span data-ttu-id="64214-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="64214-113">String collection</span></span>|<span data-ttu-id="64214-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="64214-114">Allowed Actions</span></span>|
|<span data-ttu-id="64214-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="64214-115">notAllowedResourceActions</span></span>|<span data-ttu-id="64214-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="64214-116">String collection</span></span>|<span data-ttu-id="64214-117">Действия не разрешены.</span><span class="sxs-lookup"><span data-stu-id="64214-117">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64214-118">Связи</span><span class="sxs-lookup"><span data-stu-id="64214-118">Relationships</span></span>
<span data-ttu-id="64214-119">Нет</span><span class="sxs-lookup"><span data-stu-id="64214-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64214-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64214-120">JSON Representation</span></span>
<span data-ttu-id="64214-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64214-121">Here is a JSON representation of the resource.</span></span>
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






