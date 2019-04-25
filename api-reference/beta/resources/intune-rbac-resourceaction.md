---
title: Тип ресурса resourceAction
description: Набор разрешенных и запрещенных действий для ресурса.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4cccb0b47d0d4724ebba7a4749529ccbfe5f7f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566341"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="d1e82-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="d1e82-103">resourceAction resource type</span></span>

> <span data-ttu-id="d1e82-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1e82-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1e82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1e82-106">Набор разрешенных и запрещенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d1e82-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d1e82-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1e82-107">Properties</span></span>
|<span data-ttu-id="d1e82-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1e82-108">Property</span></span>|<span data-ttu-id="d1e82-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d1e82-109">Type</span></span>|<span data-ttu-id="d1e82-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d1e82-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1e82-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d1e82-111">allowedResourceActions</span></span>|<span data-ttu-id="d1e82-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d1e82-112">String collection</span></span>|<span data-ttu-id="d1e82-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="d1e82-113">Allowed Actions</span></span>|
|<span data-ttu-id="d1e82-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d1e82-114">notAllowedResourceActions</span></span>|<span data-ttu-id="d1e82-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d1e82-115">String collection</span></span>|<span data-ttu-id="d1e82-116">Действия не разрешены.</span><span class="sxs-lookup"><span data-stu-id="d1e82-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1e82-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="d1e82-117">Relationships</span></span>
<span data-ttu-id="d1e82-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d1e82-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1e82-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1e82-119">JSON Representation</span></span>
<span data-ttu-id="d1e82-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1e82-120">Here is a JSON representation of the resource.</span></span>
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





