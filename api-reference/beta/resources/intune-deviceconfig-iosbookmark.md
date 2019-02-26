---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9de5d95cd14931da850ab9bdaf5c581fd17f09dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174998"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="3ef5d-103">Тип ресурса Иосбукмарк</span><span class="sxs-lookup"><span data-stu-id="3ef5d-103">iosBookmark resource type</span></span>

> <span data-ttu-id="3ef5d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ef5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ef5d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ef5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ef5d-106">Закладка URL-адреса iOS</span><span class="sxs-lookup"><span data-stu-id="3ef5d-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="3ef5d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ef5d-107">Properties</span></span>
|<span data-ttu-id="3ef5d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ef5d-108">Property</span></span>|<span data-ttu-id="3ef5d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3ef5d-109">Type</span></span>|<span data-ttu-id="3ef5d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3ef5d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ef5d-111">url</span><span class="sxs-lookup"><span data-stu-id="3ef5d-111">url</span></span>|<span data-ttu-id="3ef5d-112">String</span><span class="sxs-lookup"><span data-stu-id="3ef5d-112">String</span></span>|<span data-ttu-id="3ef5d-113">URL-адрес, разрешенный для доступа</span><span class="sxs-lookup"><span data-stu-id="3ef5d-113">URL allowed to access</span></span>|
|<span data-ttu-id="3ef5d-114">Букмаркфолдер</span><span class="sxs-lookup"><span data-stu-id="3ef5d-114">bookmarkFolder</span></span>|<span data-ttu-id="3ef5d-115">String</span><span class="sxs-lookup"><span data-stu-id="3ef5d-115">String</span></span>|<span data-ttu-id="3ef5d-116">Папка, в которую следует добавить закладку в Safari</span><span class="sxs-lookup"><span data-stu-id="3ef5d-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="3ef5d-117">displayName</span><span class="sxs-lookup"><span data-stu-id="3ef5d-117">displayName</span></span>|<span data-ttu-id="3ef5d-118">Строка</span><span class="sxs-lookup"><span data-stu-id="3ef5d-118">String</span></span>|<span data-ttu-id="3ef5d-119">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="3ef5d-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ef5d-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ef5d-120">Relationships</span></span>
<span data-ttu-id="3ef5d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3ef5d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ef5d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ef5d-122">JSON Representation</span></span>
<span data-ttu-id="3ef5d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ef5d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```




