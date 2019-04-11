---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5231ccbae496e310e414c6429190e0b4d53cbaa7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782802"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="50474-103">Тип ресурса Иосбукмарк</span><span class="sxs-lookup"><span data-stu-id="50474-103">iosBookmark resource type</span></span>

> <span data-ttu-id="50474-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50474-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50474-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50474-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50474-106">Закладка URL-адреса iOS</span><span class="sxs-lookup"><span data-stu-id="50474-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="50474-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="50474-107">Properties</span></span>
|<span data-ttu-id="50474-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="50474-108">Property</span></span>|<span data-ttu-id="50474-109">Тип</span><span class="sxs-lookup"><span data-stu-id="50474-109">Type</span></span>|<span data-ttu-id="50474-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50474-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50474-111">url</span><span class="sxs-lookup"><span data-stu-id="50474-111">url</span></span>|<span data-ttu-id="50474-112">String</span><span class="sxs-lookup"><span data-stu-id="50474-112">String</span></span>|<span data-ttu-id="50474-113">URL-адрес, разрешенный для доступа</span><span class="sxs-lookup"><span data-stu-id="50474-113">URL allowed to access</span></span>|
|<span data-ttu-id="50474-114">Букмаркфолдер</span><span class="sxs-lookup"><span data-stu-id="50474-114">bookmarkFolder</span></span>|<span data-ttu-id="50474-115">String</span><span class="sxs-lookup"><span data-stu-id="50474-115">String</span></span>|<span data-ttu-id="50474-116">Папка, в которую следует добавить закладку в Safari</span><span class="sxs-lookup"><span data-stu-id="50474-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="50474-117">displayName</span><span class="sxs-lookup"><span data-stu-id="50474-117">displayName</span></span>|<span data-ttu-id="50474-118">String</span><span class="sxs-lookup"><span data-stu-id="50474-118">String</span></span>|<span data-ttu-id="50474-119">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="50474-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="50474-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="50474-120">Relationships</span></span>
<span data-ttu-id="50474-121">Нет</span><span class="sxs-lookup"><span data-stu-id="50474-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50474-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50474-122">JSON Representation</span></span>
<span data-ttu-id="50474-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50474-123">Here is a JSON representation of the resource.</span></span>
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





