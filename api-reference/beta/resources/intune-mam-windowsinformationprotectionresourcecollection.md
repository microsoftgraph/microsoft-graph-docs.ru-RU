---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f5a31f85b70095975d1692e2a0aff175df12512
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940570"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="9d89c-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="9d89c-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="9d89c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d89c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d89c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d89c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d89c-106">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="9d89c-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="9d89c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d89c-107">Properties</span></span>
|<span data-ttu-id="9d89c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d89c-108">Property</span></span>|<span data-ttu-id="9d89c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9d89c-109">Type</span></span>|<span data-ttu-id="9d89c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d89c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d89c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9d89c-111">displayName</span></span>|<span data-ttu-id="9d89c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="9d89c-112">String</span></span>|<span data-ttu-id="9d89c-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="9d89c-113">Display name</span></span>|
|<span data-ttu-id="9d89c-114">resources</span><span class="sxs-lookup"><span data-stu-id="9d89c-114">resources</span></span>|<span data-ttu-id="9d89c-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9d89c-115">String collection</span></span>|<span data-ttu-id="9d89c-116">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="9d89c-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d89c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="9d89c-117">Relationships</span></span>
<span data-ttu-id="9d89c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9d89c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d89c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d89c-119">JSON Representation</span></span>
<span data-ttu-id="9d89c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d89c-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




