---
title: Тип ресурса settingSource
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d9a44dfbec0b9d0b7d9d06481c6ac25a12f66e0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709896"
---
# <a name="settingsource-resource-type"></a><span data-ttu-id="ab209-103">Тип ресурса settingSource</span><span class="sxs-lookup"><span data-stu-id="ab209-103">settingSource resource type</span></span>

<span data-ttu-id="ab209-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab209-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab209-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab209-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab209-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab209-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab209-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ab209-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ab209-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab209-108">Properties</span></span>
|<span data-ttu-id="ab209-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab209-109">Property</span></span>|<span data-ttu-id="ab209-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ab209-110">Type</span></span>|<span data-ttu-id="ab209-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab209-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab209-112">id</span><span class="sxs-lookup"><span data-stu-id="ab209-112">id</span></span>|<span data-ttu-id="ab209-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ab209-113">String</span></span>|<span data-ttu-id="ab209-114">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ab209-114">Not yet documented</span></span>|
|<span data-ttu-id="ab209-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ab209-115">displayName</span></span>|<span data-ttu-id="ab209-116">Строка</span><span class="sxs-lookup"><span data-stu-id="ab209-116">String</span></span>|<span data-ttu-id="ab209-117">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ab209-117">Not yet documented</span></span>|
|<span data-ttu-id="ab209-118">sourceType</span><span class="sxs-lookup"><span data-stu-id="ab209-118">sourceType</span></span>|[<span data-ttu-id="ab209-119">settingSourceType</span><span class="sxs-lookup"><span data-stu-id="ab209-119">settingSourceType</span></span>](../resources/intune-shared-settingsourcetype.md)|<span data-ttu-id="ab209-120">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ab209-120">Not yet documented.</span></span> <span data-ttu-id="ab209-121">Возможные значения: `deviceConfiguration`, `deviceIntent`.</span><span class="sxs-lookup"><span data-stu-id="ab209-121">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab209-122">Связи</span><span class="sxs-lookup"><span data-stu-id="ab209-122">Relationships</span></span>
<span data-ttu-id="ab209-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ab209-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab209-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab209-124">JSON Representation</span></span>
<span data-ttu-id="ab209-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab209-125">Here is a JSON representation of the resource.</span></span>
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





