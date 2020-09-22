---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e49aa085eb0cf23384bbed739235df46e5da1f72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978176"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="9cbd6-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="9cbd6-103">omaSetting resource type</span></span>

<span data-ttu-id="9cbd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cbd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cbd6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cbd6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cbd6-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="9cbd6-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9cbd6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cbd6-107">Properties</span></span>
|<span data-ttu-id="9cbd6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cbd6-108">Property</span></span>|<span data-ttu-id="9cbd6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9cbd6-109">Type</span></span>|<span data-ttu-id="9cbd6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9cbd6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cbd6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9cbd6-111">displayName</span></span>|<span data-ttu-id="9cbd6-112">String</span><span class="sxs-lookup"><span data-stu-id="9cbd6-112">String</span></span>|<span data-ttu-id="9cbd6-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="9cbd6-113">Display Name.</span></span>|
|<span data-ttu-id="9cbd6-114">description</span><span class="sxs-lookup"><span data-stu-id="9cbd6-114">description</span></span>|<span data-ttu-id="9cbd6-115">String</span><span class="sxs-lookup"><span data-stu-id="9cbd6-115">String</span></span>|<span data-ttu-id="9cbd6-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="9cbd6-116">Description.</span></span>|
|<span data-ttu-id="9cbd6-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="9cbd6-117">omaUri</span></span>|<span data-ttu-id="9cbd6-118">String</span><span class="sxs-lookup"><span data-stu-id="9cbd6-118">String</span></span>|<span data-ttu-id="9cbd6-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="9cbd6-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cbd6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="9cbd6-120">Relationships</span></span>
<span data-ttu-id="9cbd6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="9cbd6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cbd6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cbd6-122">JSON Representation</span></span>
<span data-ttu-id="9cbd6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cbd6-123">Here is a JSON representation of the resource.</span></span>
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









