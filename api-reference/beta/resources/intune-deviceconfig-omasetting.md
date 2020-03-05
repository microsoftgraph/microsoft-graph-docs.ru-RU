---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 411e3909a71d94be2c6086e9a00616245fca062b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525987"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="c3be5-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="c3be5-103">omaSetting resource type</span></span>

<span data-ttu-id="c3be5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c3be5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3be5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3be5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3be5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3be5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3be5-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="c3be5-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c3be5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3be5-108">Properties</span></span>
|<span data-ttu-id="c3be5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3be5-109">Property</span></span>|<span data-ttu-id="c3be5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c3be5-110">Type</span></span>|<span data-ttu-id="c3be5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3be5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3be5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c3be5-112">displayName</span></span>|<span data-ttu-id="c3be5-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c3be5-113">String</span></span>|<span data-ttu-id="c3be5-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c3be5-114">Display Name.</span></span>|
|<span data-ttu-id="c3be5-115">description</span><span class="sxs-lookup"><span data-stu-id="c3be5-115">description</span></span>|<span data-ttu-id="c3be5-116">String</span><span class="sxs-lookup"><span data-stu-id="c3be5-116">String</span></span>|<span data-ttu-id="c3be5-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="c3be5-117">Description.</span></span>|
|<span data-ttu-id="c3be5-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="c3be5-118">omaUri</span></span>|<span data-ttu-id="c3be5-119">String</span><span class="sxs-lookup"><span data-stu-id="c3be5-119">String</span></span>|<span data-ttu-id="c3be5-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="c3be5-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3be5-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c3be5-121">Relationships</span></span>
<span data-ttu-id="c3be5-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c3be5-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3be5-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3be5-123">JSON Representation</span></span>
<span data-ttu-id="c3be5-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3be5-124">Here is a JSON representation of the resource.</span></span>
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



