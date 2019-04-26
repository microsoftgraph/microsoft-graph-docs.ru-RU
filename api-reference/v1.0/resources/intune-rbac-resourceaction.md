---
title: Тип ресурса resourceAction
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a48d09d8aeadc9a5d60559d25a4bdcc322d10f21
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553892"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="4d8b6-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="4d8b6-103">resourceAction resource type</span></span>

> <span data-ttu-id="4d8b6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d8b6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d8b6-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4d8b6-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4d8b6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d8b6-106">Properties</span></span>
|<span data-ttu-id="4d8b6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d8b6-107">Property</span></span>|<span data-ttu-id="4d8b6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4d8b6-108">Type</span></span>|<span data-ttu-id="4d8b6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4d8b6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d8b6-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="4d8b6-110">allowedResourceActions</span></span>|<span data-ttu-id="4d8b6-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4d8b6-111">String collection</span></span>|<span data-ttu-id="4d8b6-112">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="4d8b6-112">Allowed Actions</span></span>|
|<span data-ttu-id="4d8b6-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="4d8b6-113">notAllowedResourceActions</span></span>|<span data-ttu-id="4d8b6-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4d8b6-114">String collection</span></span>|<span data-ttu-id="4d8b6-115">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="4d8b6-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d8b6-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="4d8b6-116">Relationships</span></span>
<span data-ttu-id="4d8b6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4d8b6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d8b6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d8b6-118">JSON Representation</span></span>
<span data-ttu-id="4d8b6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d8b6-119">Here is a JSON representation of the resource.</span></span>
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



