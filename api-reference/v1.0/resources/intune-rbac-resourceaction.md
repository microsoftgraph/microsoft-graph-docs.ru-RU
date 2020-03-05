---
title: Тип ресурса resourceAction
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae06b047fc93f09bd2b797a4eeaa296d232a0b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447964"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="dd6e2-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="dd6e2-103">resourceAction resource type</span></span>

<span data-ttu-id="dd6e2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd6e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd6e2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd6e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd6e2-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dd6e2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="dd6e2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd6e2-107">Properties</span></span>
|<span data-ttu-id="dd6e2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd6e2-108">Property</span></span>|<span data-ttu-id="dd6e2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dd6e2-109">Type</span></span>|<span data-ttu-id="dd6e2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dd6e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd6e2-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="dd6e2-111">allowedResourceActions</span></span>|<span data-ttu-id="dd6e2-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dd6e2-112">String collection</span></span>|<span data-ttu-id="dd6e2-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="dd6e2-113">Allowed Actions</span></span>|
|<span data-ttu-id="dd6e2-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="dd6e2-114">notAllowedResourceActions</span></span>|<span data-ttu-id="dd6e2-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dd6e2-115">String collection</span></span>|<span data-ttu-id="dd6e2-116">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="dd6e2-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd6e2-117">Связи</span><span class="sxs-lookup"><span data-stu-id="dd6e2-117">Relationships</span></span>
<span data-ttu-id="dd6e2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="dd6e2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd6e2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd6e2-119">JSON Representation</span></span>
<span data-ttu-id="dd6e2-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd6e2-120">Here is a JSON representation of the resource.</span></span>
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




