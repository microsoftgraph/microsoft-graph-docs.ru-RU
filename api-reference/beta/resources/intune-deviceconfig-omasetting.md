---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fdf74ba7e8932ce06bca83d88336239c2abcacf4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411038"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="c6330-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="c6330-103">omaSetting resource type</span></span>

> <span data-ttu-id="c6330-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6330-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c6330-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6330-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6330-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6330-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6330-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="c6330-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c6330-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6330-108">Properties</span></span>
|<span data-ttu-id="c6330-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6330-109">Property</span></span>|<span data-ttu-id="c6330-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c6330-110">Type</span></span>|<span data-ttu-id="c6330-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c6330-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6330-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c6330-112">displayName</span></span>|<span data-ttu-id="c6330-113">String</span><span class="sxs-lookup"><span data-stu-id="c6330-113">String</span></span>|<span data-ttu-id="c6330-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c6330-114">Display Name.</span></span>|
|<span data-ttu-id="c6330-115">description</span><span class="sxs-lookup"><span data-stu-id="c6330-115">description</span></span>|<span data-ttu-id="c6330-116">String</span><span class="sxs-lookup"><span data-stu-id="c6330-116">String</span></span>|<span data-ttu-id="c6330-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="c6330-117">Description.</span></span>|
|<span data-ttu-id="c6330-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="c6330-118">omaUri</span></span>|<span data-ttu-id="c6330-119">String</span><span class="sxs-lookup"><span data-stu-id="c6330-119">String</span></span>|<span data-ttu-id="c6330-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="c6330-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6330-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c6330-121">Relationships</span></span>
<span data-ttu-id="c6330-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c6330-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6330-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6330-123">JSON Representation</span></span>
<span data-ttu-id="c6330-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6330-124">Here is a JSON representation of the resource.</span></span>
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




