---
title: Тип ресурса vppTokenActionResult
description: Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f9146b98288a7ed5a7f6de944cc832ddc71f9179
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527696"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="6b672-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="6b672-103">vppTokenActionResult resource type</span></span>

<span data-ttu-id="6b672-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6b672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b672-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b672-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b672-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b672-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b672-107">Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6b672-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="6b672-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b672-108">Properties</span></span>
|<span data-ttu-id="6b672-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b672-109">Property</span></span>|<span data-ttu-id="6b672-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6b672-110">Type</span></span>|<span data-ttu-id="6b672-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b672-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b672-112">actionName</span><span class="sxs-lookup"><span data-stu-id="6b672-112">actionName</span></span>|<span data-ttu-id="6b672-113">String</span><span class="sxs-lookup"><span data-stu-id="6b672-113">String</span></span>|<span data-ttu-id="6b672-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="6b672-114">Action name</span></span>|
|<span data-ttu-id="6b672-115">actionState</span><span class="sxs-lookup"><span data-stu-id="6b672-115">actionState</span></span>|[<span data-ttu-id="6b672-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6b672-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6b672-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="6b672-117">State of the action.</span></span> <span data-ttu-id="6b672-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6b672-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6b672-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6b672-119">startDateTime</span></span>|<span data-ttu-id="6b672-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b672-120">DateTimeOffset</span></span>|<span data-ttu-id="6b672-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="6b672-121">Time the action was initiated</span></span>|
|<span data-ttu-id="6b672-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b672-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="6b672-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b672-123">DateTimeOffset</span></span>|<span data-ttu-id="6b672-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="6b672-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b672-125">Связи</span><span class="sxs-lookup"><span data-stu-id="6b672-125">Relationships</span></span>
<span data-ttu-id="6b672-126">Нет</span><span class="sxs-lookup"><span data-stu-id="6b672-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b672-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b672-127">JSON Representation</span></span>
<span data-ttu-id="6b672-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b672-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



