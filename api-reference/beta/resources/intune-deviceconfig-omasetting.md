---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f53e50bdf3584ab7f34afedbd938ad0749eb23b6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788487"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="d8552-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="d8552-103">omaSetting resource type</span></span>

> <span data-ttu-id="d8552-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8552-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8552-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8552-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8552-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d8552-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d8552-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8552-107">Properties</span></span>
|<span data-ttu-id="d8552-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8552-108">Property</span></span>|<span data-ttu-id="d8552-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d8552-109">Type</span></span>|<span data-ttu-id="d8552-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d8552-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8552-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d8552-111">displayName</span></span>|<span data-ttu-id="d8552-112">Строка</span><span class="sxs-lookup"><span data-stu-id="d8552-112">String</span></span>|<span data-ttu-id="d8552-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d8552-113">Display Name.</span></span>|
|<span data-ttu-id="d8552-114">description</span><span class="sxs-lookup"><span data-stu-id="d8552-114">description</span></span>|<span data-ttu-id="d8552-115">String</span><span class="sxs-lookup"><span data-stu-id="d8552-115">String</span></span>|<span data-ttu-id="d8552-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="d8552-116">Description.</span></span>|
|<span data-ttu-id="d8552-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="d8552-117">omaUri</span></span>|<span data-ttu-id="d8552-118">String</span><span class="sxs-lookup"><span data-stu-id="d8552-118">String</span></span>|<span data-ttu-id="d8552-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="d8552-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8552-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d8552-120">Relationships</span></span>
<span data-ttu-id="d8552-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d8552-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8552-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8552-122">JSON Representation</span></span>
<span data-ttu-id="d8552-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8552-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



