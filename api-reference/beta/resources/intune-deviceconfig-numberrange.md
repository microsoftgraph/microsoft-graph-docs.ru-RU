---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbc802ef17c6e83d10f93661e7aca05cdc2cee02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969984"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="69847-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="69847-103">numberRange resource type</span></span>

> <span data-ttu-id="69847-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69847-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69847-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69847-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69847-106">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="69847-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="69847-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="69847-107">Properties</span></span>
|<span data-ttu-id="69847-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="69847-108">Property</span></span>|<span data-ttu-id="69847-109">Тип</span><span class="sxs-lookup"><span data-stu-id="69847-109">Type</span></span>|<span data-ttu-id="69847-110">Описание</span><span class="sxs-lookup"><span data-stu-id="69847-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69847-111">Ловернумбер</span><span class="sxs-lookup"><span data-stu-id="69847-111">lowerNumber</span></span>|<span data-ttu-id="69847-112">Int32</span><span class="sxs-lookup"><span data-stu-id="69847-112">Int32</span></span>|<span data-ttu-id="69847-113">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="69847-113">Lower number.</span></span>|
|<span data-ttu-id="69847-114">Уппернумбер</span><span class="sxs-lookup"><span data-stu-id="69847-114">upperNumber</span></span>|<span data-ttu-id="69847-115">Int32</span><span class="sxs-lookup"><span data-stu-id="69847-115">Int32</span></span>|<span data-ttu-id="69847-116">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="69847-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69847-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="69847-117">Relationships</span></span>
<span data-ttu-id="69847-118">Нет</span><span class="sxs-lookup"><span data-stu-id="69847-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69847-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69847-119">JSON Representation</span></span>
<span data-ttu-id="69847-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69847-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```





