---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb647b44f477efc5b3b24778653d300d0b994b7b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272250"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="bda90-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="bda90-103">windowsInformationProtectionResourceCollection resource type</span></span>

<span data-ttu-id="bda90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bda90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bda90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bda90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bda90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bda90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bda90-107">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="bda90-107">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="bda90-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bda90-108">Properties</span></span>
|<span data-ttu-id="bda90-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bda90-109">Property</span></span>|<span data-ttu-id="bda90-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bda90-110">Type</span></span>|<span data-ttu-id="bda90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bda90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bda90-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bda90-112">displayName</span></span>|<span data-ttu-id="bda90-113">String</span><span class="sxs-lookup"><span data-stu-id="bda90-113">String</span></span>|<span data-ttu-id="bda90-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="bda90-114">Display name</span></span>|
|<span data-ttu-id="bda90-115">resources</span><span class="sxs-lookup"><span data-stu-id="bda90-115">resources</span></span>|<span data-ttu-id="bda90-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bda90-116">String collection</span></span>|<span data-ttu-id="bda90-117">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="bda90-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="bda90-118">Связи</span><span class="sxs-lookup"><span data-stu-id="bda90-118">Relationships</span></span>
<span data-ttu-id="bda90-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bda90-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bda90-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bda90-120">JSON Representation</span></span>
<span data-ttu-id="bda90-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bda90-121">Here is a JSON representation of the resource.</span></span>
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




