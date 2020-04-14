---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bfd4c72bc6018a4b49bcc20c0c1abd953052e471
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402038"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="662eb-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="662eb-103">omaSetting resource type</span></span>

<span data-ttu-id="662eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="662eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="662eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="662eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="662eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="662eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="662eb-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="662eb-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="662eb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="662eb-108">Properties</span></span>
|<span data-ttu-id="662eb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="662eb-109">Property</span></span>|<span data-ttu-id="662eb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="662eb-110">Type</span></span>|<span data-ttu-id="662eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="662eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="662eb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="662eb-112">displayName</span></span>|<span data-ttu-id="662eb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="662eb-113">String</span></span>|<span data-ttu-id="662eb-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="662eb-114">Display Name.</span></span>|
|<span data-ttu-id="662eb-115">description</span><span class="sxs-lookup"><span data-stu-id="662eb-115">description</span></span>|<span data-ttu-id="662eb-116">String</span><span class="sxs-lookup"><span data-stu-id="662eb-116">String</span></span>|<span data-ttu-id="662eb-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="662eb-117">Description.</span></span>|
|<span data-ttu-id="662eb-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="662eb-118">omaUri</span></span>|<span data-ttu-id="662eb-119">String</span><span class="sxs-lookup"><span data-stu-id="662eb-119">String</span></span>|<span data-ttu-id="662eb-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="662eb-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="662eb-121">Связи</span><span class="sxs-lookup"><span data-stu-id="662eb-121">Relationships</span></span>
<span data-ttu-id="662eb-122">Нет</span><span class="sxs-lookup"><span data-stu-id="662eb-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="662eb-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="662eb-123">JSON Representation</span></span>
<span data-ttu-id="662eb-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="662eb-124">Here is a JSON representation of the resource.</span></span>
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



