---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88b5a45d466a50f3bdc9a5b53790ff5c10f53904
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024047"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="d84cb-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="d84cb-103">omaSetting resource type</span></span>

<span data-ttu-id="d84cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d84cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d84cb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d84cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d84cb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d84cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d84cb-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d84cb-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d84cb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d84cb-108">Properties</span></span>
|<span data-ttu-id="d84cb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d84cb-109">Property</span></span>|<span data-ttu-id="d84cb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d84cb-110">Type</span></span>|<span data-ttu-id="d84cb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d84cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d84cb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d84cb-112">displayName</span></span>|<span data-ttu-id="d84cb-113">String</span><span class="sxs-lookup"><span data-stu-id="d84cb-113">String</span></span>|<span data-ttu-id="d84cb-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d84cb-114">Display Name.</span></span>|
|<span data-ttu-id="d84cb-115">description</span><span class="sxs-lookup"><span data-stu-id="d84cb-115">description</span></span>|<span data-ttu-id="d84cb-116">String</span><span class="sxs-lookup"><span data-stu-id="d84cb-116">String</span></span>|<span data-ttu-id="d84cb-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="d84cb-117">Description.</span></span>|
|<span data-ttu-id="d84cb-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="d84cb-118">omaUri</span></span>|<span data-ttu-id="d84cb-119">String</span><span class="sxs-lookup"><span data-stu-id="d84cb-119">String</span></span>|<span data-ttu-id="d84cb-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="d84cb-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d84cb-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="d84cb-121">Relationships</span></span>
<span data-ttu-id="d84cb-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d84cb-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d84cb-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d84cb-123">JSON Representation</span></span>
<span data-ttu-id="d84cb-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d84cb-124">Here is a JSON representation of the resource.</span></span>
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






