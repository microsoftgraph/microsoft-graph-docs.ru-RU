---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d0a69c10f1f0075caee48276bdbc37f6d616f22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549554"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="91287-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="91287-103">omaSetting resource type</span></span>

> <span data-ttu-id="91287-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91287-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91287-105">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="91287-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="91287-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="91287-106">Properties</span></span>
|<span data-ttu-id="91287-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="91287-107">Property</span></span>|<span data-ttu-id="91287-108">Тип</span><span class="sxs-lookup"><span data-stu-id="91287-108">Type</span></span>|<span data-ttu-id="91287-109">Описание</span><span class="sxs-lookup"><span data-stu-id="91287-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91287-110">displayName</span><span class="sxs-lookup"><span data-stu-id="91287-110">displayName</span></span>|<span data-ttu-id="91287-111">String</span><span class="sxs-lookup"><span data-stu-id="91287-111">String</span></span>|<span data-ttu-id="91287-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="91287-112">Display Name.</span></span>|
|<span data-ttu-id="91287-113">description</span><span class="sxs-lookup"><span data-stu-id="91287-113">description</span></span>|<span data-ttu-id="91287-114">String</span><span class="sxs-lookup"><span data-stu-id="91287-114">String</span></span>|<span data-ttu-id="91287-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="91287-115">Description.</span></span>|
|<span data-ttu-id="91287-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="91287-116">omaUri</span></span>|<span data-ttu-id="91287-117">String</span><span class="sxs-lookup"><span data-stu-id="91287-117">String</span></span>|<span data-ttu-id="91287-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="91287-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91287-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="91287-119">Relationships</span></span>
<span data-ttu-id="91287-120">Нет</span><span class="sxs-lookup"><span data-stu-id="91287-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91287-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91287-121">JSON Representation</span></span>
<span data-ttu-id="91287-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91287-122">Here is a JSON representation of the resource.</span></span>
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



