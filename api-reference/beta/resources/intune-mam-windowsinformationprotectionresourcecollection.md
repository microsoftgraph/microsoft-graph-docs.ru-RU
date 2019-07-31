---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f8f21fcdf33676520301dbaeccefc12696375cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967842"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="f9ed5-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="f9ed5-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="f9ed5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ed5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9ed5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9ed5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ed5-106">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="f9ed5-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f9ed5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9ed5-107">Properties</span></span>
|<span data-ttu-id="f9ed5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9ed5-108">Property</span></span>|<span data-ttu-id="f9ed5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f9ed5-109">Type</span></span>|<span data-ttu-id="f9ed5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f9ed5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9ed5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f9ed5-111">displayName</span></span>|<span data-ttu-id="f9ed5-112">String</span><span class="sxs-lookup"><span data-stu-id="f9ed5-112">String</span></span>|<span data-ttu-id="f9ed5-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="f9ed5-113">Display name</span></span>|
|<span data-ttu-id="f9ed5-114">resources</span><span class="sxs-lookup"><span data-stu-id="f9ed5-114">resources</span></span>|<span data-ttu-id="f9ed5-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f9ed5-115">String collection</span></span>|<span data-ttu-id="f9ed5-116">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="f9ed5-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9ed5-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="f9ed5-117">Relationships</span></span>
<span data-ttu-id="f9ed5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f9ed5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9ed5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9ed5-119">JSON Representation</span></span>
<span data-ttu-id="f9ed5-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9ed5-120">Here is a JSON representation of the resource.</span></span>
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





