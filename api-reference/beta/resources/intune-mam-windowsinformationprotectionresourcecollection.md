---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5a303ad0b05813a4e44dc2208ff1b8692242d88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561847"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="f85d8-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="f85d8-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="f85d8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f85d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f85d8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f85d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f85d8-106">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="f85d8-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f85d8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f85d8-107">Properties</span></span>
|<span data-ttu-id="f85d8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f85d8-108">Property</span></span>|<span data-ttu-id="f85d8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f85d8-109">Type</span></span>|<span data-ttu-id="f85d8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f85d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f85d8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f85d8-111">displayName</span></span>|<span data-ttu-id="f85d8-112">String</span><span class="sxs-lookup"><span data-stu-id="f85d8-112">String</span></span>|<span data-ttu-id="f85d8-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="f85d8-113">Display name</span></span>|
|<span data-ttu-id="f85d8-114">resources</span><span class="sxs-lookup"><span data-stu-id="f85d8-114">resources</span></span>|<span data-ttu-id="f85d8-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f85d8-115">String collection</span></span>|<span data-ttu-id="f85d8-116">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="f85d8-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="f85d8-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="f85d8-117">Relationships</span></span>
<span data-ttu-id="f85d8-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f85d8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f85d8-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f85d8-119">JSON Representation</span></span>
<span data-ttu-id="f85d8-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f85d8-120">Here is a JSON representation of the resource.</span></span>
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





