---
title: Тип ресурса resourceAction
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94a0ce30dc6e9607aa1531e7421af6b7a5500939
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870736"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="3c430-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="3c430-103">resourceAction resource type</span></span>

> <span data-ttu-id="3c430-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3c430-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c430-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3c430-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3c430-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c430-106">Properties</span></span>
|<span data-ttu-id="3c430-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c430-107">Property</span></span>|<span data-ttu-id="3c430-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3c430-108">Type</span></span>|<span data-ttu-id="3c430-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3c430-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c430-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="3c430-110">allowedResourceActions</span></span>|<span data-ttu-id="3c430-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3c430-111">String collection</span></span>|<span data-ttu-id="3c430-112">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="3c430-112">Allowed Actions</span></span>|
|<span data-ttu-id="3c430-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="3c430-113">notAllowedResourceActions</span></span>|<span data-ttu-id="3c430-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3c430-114">String collection</span></span>|<span data-ttu-id="3c430-115">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="3c430-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c430-116">Связи</span><span class="sxs-lookup"><span data-stu-id="3c430-116">Relationships</span></span>
<span data-ttu-id="3c430-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3c430-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c430-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c430-118">JSON Representation</span></span>
<span data-ttu-id="3c430-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c430-119">Here is a JSON representation of the resource.</span></span>
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



