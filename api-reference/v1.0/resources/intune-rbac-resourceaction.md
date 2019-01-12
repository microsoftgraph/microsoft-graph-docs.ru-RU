---
title: Тип ресурса resourceAction
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1db2a1db2c76829ddd39438ed40cd1086fe4e17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932715"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="ccc66-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="ccc66-103">resourceAction resource type</span></span>

> <span data-ttu-id="ccc66-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ccc66-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ccc66-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ccc66-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ccc66-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ccc66-106">Properties</span></span>
|<span data-ttu-id="ccc66-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccc66-107">Property</span></span>|<span data-ttu-id="ccc66-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ccc66-108">Type</span></span>|<span data-ttu-id="ccc66-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ccc66-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccc66-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="ccc66-110">allowedResourceActions</span></span>|<span data-ttu-id="ccc66-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ccc66-111">String collection</span></span>|<span data-ttu-id="ccc66-112">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="ccc66-112">Allowed Actions</span></span>|
|<span data-ttu-id="ccc66-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="ccc66-113">notAllowedResourceActions</span></span>|<span data-ttu-id="ccc66-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ccc66-114">String collection</span></span>|<span data-ttu-id="ccc66-115">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="ccc66-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccc66-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ccc66-116">Relationships</span></span>
<span data-ttu-id="ccc66-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ccc66-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ccc66-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ccc66-118">JSON Representation</span></span>
<span data-ttu-id="ccc66-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccc66-119">Here is a JSON representation of the resource.</span></span>
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



