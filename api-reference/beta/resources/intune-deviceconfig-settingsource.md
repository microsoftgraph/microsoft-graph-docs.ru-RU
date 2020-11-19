---
title: Тип ресурса settingSource
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f0ebdabfbcb77a650580e92aaa3af14e2e9035a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293754"
---
# <a name="settingsource-resource-type"></a><span data-ttu-id="88dc3-103">Тип ресурса settingSource</span><span class="sxs-lookup"><span data-stu-id="88dc3-103">settingSource resource type</span></span>

<span data-ttu-id="88dc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88dc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88dc3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88dc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88dc3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88dc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88dc3-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="88dc3-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="88dc3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="88dc3-108">Properties</span></span>
|<span data-ttu-id="88dc3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="88dc3-109">Property</span></span>|<span data-ttu-id="88dc3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="88dc3-110">Type</span></span>|<span data-ttu-id="88dc3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88dc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88dc3-112">id</span><span class="sxs-lookup"><span data-stu-id="88dc3-112">id</span></span>|<span data-ttu-id="88dc3-113">String</span><span class="sxs-lookup"><span data-stu-id="88dc3-113">String</span></span>|<span data-ttu-id="88dc3-114">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="88dc3-114">Not yet documented</span></span>|
|<span data-ttu-id="88dc3-115">displayName</span><span class="sxs-lookup"><span data-stu-id="88dc3-115">displayName</span></span>|<span data-ttu-id="88dc3-116">String</span><span class="sxs-lookup"><span data-stu-id="88dc3-116">String</span></span>|<span data-ttu-id="88dc3-117">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="88dc3-117">Not yet documented</span></span>|
|<span data-ttu-id="88dc3-118">sourceType</span><span class="sxs-lookup"><span data-stu-id="88dc3-118">sourceType</span></span>|[<span data-ttu-id="88dc3-119">settingSourceType</span><span class="sxs-lookup"><span data-stu-id="88dc3-119">settingSourceType</span></span>](../resources/intune-shared-settingsourcetype.md)|<span data-ttu-id="88dc3-120">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="88dc3-120">Not yet documented.</span></span> <span data-ttu-id="88dc3-121">Возможные значения: `deviceConfiguration`, `deviceIntent`.</span><span class="sxs-lookup"><span data-stu-id="88dc3-121">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88dc3-122">Связи</span><span class="sxs-lookup"><span data-stu-id="88dc3-122">Relationships</span></span>
<span data-ttu-id="88dc3-123">Нет</span><span class="sxs-lookup"><span data-stu-id="88dc3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88dc3-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88dc3-124">JSON Representation</span></span>
<span data-ttu-id="88dc3-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88dc3-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.settingSource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingSource",
  "id": "String (identifier)",
  "displayName": "String",
  "sourceType": "String"
}
```




