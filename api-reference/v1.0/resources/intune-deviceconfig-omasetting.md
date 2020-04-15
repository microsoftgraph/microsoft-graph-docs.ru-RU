---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0172d3cb6955df6e154758750fdc87aef2789292
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473080"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="5f57f-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="5f57f-103">omaSetting resource type</span></span>

<span data-ttu-id="5f57f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f57f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f57f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f57f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f57f-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="5f57f-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="5f57f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f57f-107">Properties</span></span>
|<span data-ttu-id="5f57f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f57f-108">Property</span></span>|<span data-ttu-id="5f57f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5f57f-109">Type</span></span>|<span data-ttu-id="5f57f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f57f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f57f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5f57f-111">displayName</span></span>|<span data-ttu-id="5f57f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5f57f-112">String</span></span>|<span data-ttu-id="5f57f-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="5f57f-113">Display Name.</span></span>|
|<span data-ttu-id="5f57f-114">description</span><span class="sxs-lookup"><span data-stu-id="5f57f-114">description</span></span>|<span data-ttu-id="5f57f-115">String</span><span class="sxs-lookup"><span data-stu-id="5f57f-115">String</span></span>|<span data-ttu-id="5f57f-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="5f57f-116">Description.</span></span>|
|<span data-ttu-id="5f57f-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="5f57f-117">omaUri</span></span>|<span data-ttu-id="5f57f-118">String</span><span class="sxs-lookup"><span data-stu-id="5f57f-118">String</span></span>|<span data-ttu-id="5f57f-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="5f57f-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f57f-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="5f57f-120">Relationships</span></span>
<span data-ttu-id="5f57f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5f57f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f57f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f57f-122">JSON Representation</span></span>
<span data-ttu-id="5f57f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f57f-123">Here is a JSON representation of the resource.</span></span>
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







