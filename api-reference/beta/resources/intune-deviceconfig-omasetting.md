---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fab80ad06fb5654578f29b92e3b0f3aa9c09abdb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143850"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="24434-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="24434-103">omaSetting resource type</span></span>

> <span data-ttu-id="24434-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24434-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24434-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24434-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24434-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="24434-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="24434-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="24434-107">Properties</span></span>
|<span data-ttu-id="24434-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="24434-108">Property</span></span>|<span data-ttu-id="24434-109">Тип</span><span class="sxs-lookup"><span data-stu-id="24434-109">Type</span></span>|<span data-ttu-id="24434-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24434-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24434-111">displayName</span><span class="sxs-lookup"><span data-stu-id="24434-111">displayName</span></span>|<span data-ttu-id="24434-112">String</span><span class="sxs-lookup"><span data-stu-id="24434-112">String</span></span>|<span data-ttu-id="24434-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="24434-113">Display Name.</span></span>|
|<span data-ttu-id="24434-114">description</span><span class="sxs-lookup"><span data-stu-id="24434-114">description</span></span>|<span data-ttu-id="24434-115">String</span><span class="sxs-lookup"><span data-stu-id="24434-115">String</span></span>|<span data-ttu-id="24434-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="24434-116">Description.</span></span>|
|<span data-ttu-id="24434-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="24434-117">omaUri</span></span>|<span data-ttu-id="24434-118">String</span><span class="sxs-lookup"><span data-stu-id="24434-118">String</span></span>|<span data-ttu-id="24434-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="24434-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24434-120">Связи</span><span class="sxs-lookup"><span data-stu-id="24434-120">Relationships</span></span>
<span data-ttu-id="24434-121">Нет</span><span class="sxs-lookup"><span data-stu-id="24434-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24434-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24434-122">JSON Representation</span></span>
<span data-ttu-id="24434-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24434-123">Here is a JSON representation of the resource.</span></span>
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




