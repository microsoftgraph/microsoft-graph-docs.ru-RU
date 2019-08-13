---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1cb8a58130e2e51d16393287811e2025da6778a9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368543"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="20c23-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="20c23-103">omaSetting resource type</span></span>

> <span data-ttu-id="20c23-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20c23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20c23-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20c23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20c23-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="20c23-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="20c23-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="20c23-107">Properties</span></span>
|<span data-ttu-id="20c23-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="20c23-108">Property</span></span>|<span data-ttu-id="20c23-109">Тип</span><span class="sxs-lookup"><span data-stu-id="20c23-109">Type</span></span>|<span data-ttu-id="20c23-110">Описание</span><span class="sxs-lookup"><span data-stu-id="20c23-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20c23-111">displayName</span><span class="sxs-lookup"><span data-stu-id="20c23-111">displayName</span></span>|<span data-ttu-id="20c23-112">Строка</span><span class="sxs-lookup"><span data-stu-id="20c23-112">String</span></span>|<span data-ttu-id="20c23-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="20c23-113">Display Name.</span></span>|
|<span data-ttu-id="20c23-114">description</span><span class="sxs-lookup"><span data-stu-id="20c23-114">description</span></span>|<span data-ttu-id="20c23-115">String</span><span class="sxs-lookup"><span data-stu-id="20c23-115">String</span></span>|<span data-ttu-id="20c23-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="20c23-116">Description.</span></span>|
|<span data-ttu-id="20c23-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="20c23-117">omaUri</span></span>|<span data-ttu-id="20c23-118">String</span><span class="sxs-lookup"><span data-stu-id="20c23-118">String</span></span>|<span data-ttu-id="20c23-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="20c23-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20c23-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="20c23-120">Relationships</span></span>
<span data-ttu-id="20c23-121">Нет</span><span class="sxs-lookup"><span data-stu-id="20c23-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20c23-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20c23-122">JSON Representation</span></span>
<span data-ttu-id="20c23-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20c23-123">Here is a JSON representation of the resource.</span></span>
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



