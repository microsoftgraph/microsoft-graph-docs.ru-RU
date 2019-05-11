---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c595256953928138ec140b799410f5ba43d0b3de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950972"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="282b5-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="282b5-103">omaSetting resource type</span></span>

> <span data-ttu-id="282b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="282b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="282b5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="282b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="282b5-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="282b5-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="282b5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="282b5-107">Properties</span></span>
|<span data-ttu-id="282b5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="282b5-108">Property</span></span>|<span data-ttu-id="282b5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="282b5-109">Type</span></span>|<span data-ttu-id="282b5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="282b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="282b5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="282b5-111">displayName</span></span>|<span data-ttu-id="282b5-112">Строка</span><span class="sxs-lookup"><span data-stu-id="282b5-112">String</span></span>|<span data-ttu-id="282b5-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="282b5-113">Display Name.</span></span>|
|<span data-ttu-id="282b5-114">description</span><span class="sxs-lookup"><span data-stu-id="282b5-114">description</span></span>|<span data-ttu-id="282b5-115">String</span><span class="sxs-lookup"><span data-stu-id="282b5-115">String</span></span>|<span data-ttu-id="282b5-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="282b5-116">Description.</span></span>|
|<span data-ttu-id="282b5-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="282b5-117">omaUri</span></span>|<span data-ttu-id="282b5-118">String</span><span class="sxs-lookup"><span data-stu-id="282b5-118">String</span></span>|<span data-ttu-id="282b5-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="282b5-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="282b5-120">Связи</span><span class="sxs-lookup"><span data-stu-id="282b5-120">Relationships</span></span>
<span data-ttu-id="282b5-121">Нет</span><span class="sxs-lookup"><span data-stu-id="282b5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="282b5-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="282b5-122">JSON Representation</span></span>
<span data-ttu-id="282b5-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="282b5-123">Here is a JSON representation of the resource.</span></span>
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




