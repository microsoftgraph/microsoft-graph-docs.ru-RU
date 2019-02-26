---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d0a69c10f1f0075caee48276bdbc37f6d616f22
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253381"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="55cec-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="55cec-103">omaSetting resource type</span></span>

> <span data-ttu-id="55cec-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55cec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55cec-105">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="55cec-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="55cec-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="55cec-106">Properties</span></span>
|<span data-ttu-id="55cec-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="55cec-107">Property</span></span>|<span data-ttu-id="55cec-108">Тип</span><span class="sxs-lookup"><span data-stu-id="55cec-108">Type</span></span>|<span data-ttu-id="55cec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="55cec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55cec-110">displayName</span><span class="sxs-lookup"><span data-stu-id="55cec-110">displayName</span></span>|<span data-ttu-id="55cec-111">String</span><span class="sxs-lookup"><span data-stu-id="55cec-111">String</span></span>|<span data-ttu-id="55cec-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="55cec-112">Display Name.</span></span>|
|<span data-ttu-id="55cec-113">description</span><span class="sxs-lookup"><span data-stu-id="55cec-113">description</span></span>|<span data-ttu-id="55cec-114">String</span><span class="sxs-lookup"><span data-stu-id="55cec-114">String</span></span>|<span data-ttu-id="55cec-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="55cec-115">Description.</span></span>|
|<span data-ttu-id="55cec-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="55cec-116">omaUri</span></span>|<span data-ttu-id="55cec-117">String</span><span class="sxs-lookup"><span data-stu-id="55cec-117">String</span></span>|<span data-ttu-id="55cec-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="55cec-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55cec-119">Связи</span><span class="sxs-lookup"><span data-stu-id="55cec-119">Relationships</span></span>
<span data-ttu-id="55cec-120">Нет</span><span class="sxs-lookup"><span data-stu-id="55cec-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55cec-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55cec-121">JSON Representation</span></span>
<span data-ttu-id="55cec-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55cec-122">Here is a JSON representation of the resource.</span></span>
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



