---
title: Тип ресурса resourceAction
description: Н/Д
author: tfitzmac
ms.openlocfilehash: b64c1fb0ef49c2d7c47c88137bcca8ef89f6ad67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343920"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="e7371-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="e7371-103">resourceAction resource type</span></span>

> <span data-ttu-id="e7371-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7371-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7371-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e7371-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e7371-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7371-106">Properties</span></span>
|<span data-ttu-id="e7371-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7371-107">Property</span></span>|<span data-ttu-id="e7371-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e7371-108">Type</span></span>|<span data-ttu-id="e7371-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e7371-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7371-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="e7371-110">allowedResourceActions</span></span>|<span data-ttu-id="e7371-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e7371-111">String collection</span></span>|<span data-ttu-id="e7371-112">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="e7371-112">Allowed Actions</span></span>|
|<span data-ttu-id="e7371-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="e7371-113">notAllowedResourceActions</span></span>|<span data-ttu-id="e7371-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e7371-114">String collection</span></span>|<span data-ttu-id="e7371-115">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="e7371-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7371-116">Связи</span><span class="sxs-lookup"><span data-stu-id="e7371-116">Relationships</span></span>
<span data-ttu-id="e7371-117">Нет</span><span class="sxs-lookup"><span data-stu-id="e7371-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7371-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7371-118">JSON Representation</span></span>
<span data-ttu-id="e7371-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7371-119">Here is a JSON representation of the resource.</span></span>
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



