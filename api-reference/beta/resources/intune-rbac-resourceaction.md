---
title: Тип ресурса resourceAction
description: Набор разрешенных и запрещенных действий для ресурса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b8d176b64b6eacc7fbf34a4fe5e15a88da709f2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733184"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="eac9c-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="eac9c-103">resourceAction resource type</span></span>

<span data-ttu-id="eac9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eac9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eac9c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eac9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eac9c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eac9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eac9c-107">Набор разрешенных и запрещенных действий для ресурса.</span><span class="sxs-lookup"><span data-stu-id="eac9c-107">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="eac9c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eac9c-108">Properties</span></span>
|<span data-ttu-id="eac9c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eac9c-109">Property</span></span>|<span data-ttu-id="eac9c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eac9c-110">Type</span></span>|<span data-ttu-id="eac9c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eac9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eac9c-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="eac9c-112">allowedResourceActions</span></span>|<span data-ttu-id="eac9c-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="eac9c-113">String collection</span></span>|<span data-ttu-id="eac9c-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="eac9c-114">Allowed Actions</span></span>|
|<span data-ttu-id="eac9c-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="eac9c-115">notAllowedResourceActions</span></span>|<span data-ttu-id="eac9c-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="eac9c-116">String collection</span></span>|<span data-ttu-id="eac9c-117">Действия не разрешены.</span><span class="sxs-lookup"><span data-stu-id="eac9c-117">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eac9c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="eac9c-118">Relationships</span></span>
<span data-ttu-id="eac9c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="eac9c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eac9c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eac9c-120">JSON Representation</span></span>
<span data-ttu-id="eac9c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eac9c-121">Here is a JSON representation of the resource.</span></span>
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





