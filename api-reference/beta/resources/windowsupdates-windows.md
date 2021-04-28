---
title: Тип ресурса Windows
description: Объект, который выступает в качестве контейнера для Windows функций.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3f7677f97db8d57e1fba74174df8cd848ad4f224
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067488"
---
# <a name="windows-resource-type"></a><span data-ttu-id="5ff9a-103">Тип ресурса Windows</span><span class="sxs-lookup"><span data-stu-id="5ff9a-103">windows resource type</span></span>

<span data-ttu-id="5ff9a-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="5ff9a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ff9a-105">Объект, который выступает в качестве контейнера для Windows функций.</span><span class="sxs-lookup"><span data-stu-id="5ff9a-105">Entity that acts as a container for Windows functionality.</span></span>

## <a name="properties"></a><span data-ttu-id="5ff9a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ff9a-106">Properties</span></span>
|<span data-ttu-id="5ff9a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ff9a-107">Property</span></span>|<span data-ttu-id="5ff9a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5ff9a-108">Type</span></span>|<span data-ttu-id="5ff9a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5ff9a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ff9a-110">id</span><span class="sxs-lookup"><span data-stu-id="5ff9a-110">id</span></span>|<span data-ttu-id="5ff9a-111">String</span><span class="sxs-lookup"><span data-stu-id="5ff9a-111">String</span></span>|<span data-ttu-id="5ff9a-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ff9a-112">Read-only.</span></span> <span data-ttu-id="5ff9a-113">Унаследованный от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="5ff9a-113">Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ff9a-114">Связи</span><span class="sxs-lookup"><span data-stu-id="5ff9a-114">Relationships</span></span>
|<span data-ttu-id="5ff9a-115">Связь</span><span class="sxs-lookup"><span data-stu-id="5ff9a-115">Relationship</span></span>|<span data-ttu-id="5ff9a-116">Тип</span><span class="sxs-lookup"><span data-stu-id="5ff9a-116">Type</span></span>|<span data-ttu-id="5ff9a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5ff9a-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ff9a-118">обновления</span><span class="sxs-lookup"><span data-stu-id="5ff9a-118">updates</span></span>|[<span data-ttu-id="5ff9a-119">microsoft.graph.windowsUpdates.updates</span><span class="sxs-lookup"><span data-stu-id="5ff9a-119">microsoft.graph.windowsUpdates.updates</span></span>](../resources/windowsupdates-updates.md)|<span data-ttu-id="5ff9a-120">Объект, который выступает в качестве контейнера для функциональных возможностей службы Windows обновления для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5ff9a-120">Entity that acts as a container for the functionality of the Windows Update for Business deployment service.</span></span> <span data-ttu-id="5ff9a-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ff9a-121">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ff9a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ff9a-122">JSON representation</span></span>
<span data-ttu-id="5ff9a-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ff9a-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.windows",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windows",
  "id": "String (identifier)"
}
```

