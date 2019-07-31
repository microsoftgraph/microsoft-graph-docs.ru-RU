---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9310ffe3a664b3fc02e9f498a2c5312dc6683b53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004346"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="b6c2d-103">Тип ресурса Иосбукмарк</span><span class="sxs-lookup"><span data-stu-id="b6c2d-103">iosBookmark resource type</span></span>

> <span data-ttu-id="b6c2d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6c2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6c2d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6c2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6c2d-106">Закладка URL-адреса iOS</span><span class="sxs-lookup"><span data-stu-id="b6c2d-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="b6c2d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6c2d-107">Properties</span></span>
|<span data-ttu-id="b6c2d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6c2d-108">Property</span></span>|<span data-ttu-id="b6c2d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b6c2d-109">Type</span></span>|<span data-ttu-id="b6c2d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b6c2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6c2d-111">url</span><span class="sxs-lookup"><span data-stu-id="b6c2d-111">url</span></span>|<span data-ttu-id="b6c2d-112">String</span><span class="sxs-lookup"><span data-stu-id="b6c2d-112">String</span></span>|<span data-ttu-id="b6c2d-113">URL-адрес, разрешенный для доступа</span><span class="sxs-lookup"><span data-stu-id="b6c2d-113">URL allowed to access</span></span>|
|<span data-ttu-id="b6c2d-114">Букмаркфолдер</span><span class="sxs-lookup"><span data-stu-id="b6c2d-114">bookmarkFolder</span></span>|<span data-ttu-id="b6c2d-115">String</span><span class="sxs-lookup"><span data-stu-id="b6c2d-115">String</span></span>|<span data-ttu-id="b6c2d-116">Папка, в которую следует добавить закладку в Safari</span><span class="sxs-lookup"><span data-stu-id="b6c2d-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="b6c2d-117">displayName</span><span class="sxs-lookup"><span data-stu-id="b6c2d-117">displayName</span></span>|<span data-ttu-id="b6c2d-118">String</span><span class="sxs-lookup"><span data-stu-id="b6c2d-118">String</span></span>|<span data-ttu-id="b6c2d-119">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="b6c2d-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6c2d-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="b6c2d-120">Relationships</span></span>
<span data-ttu-id="b6c2d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b6c2d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6c2d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6c2d-122">JSON Representation</span></span>
<span data-ttu-id="b6c2d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6c2d-123">Here is a JSON representation of the resource.</span></span>
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





