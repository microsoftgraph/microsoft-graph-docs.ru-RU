---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c8a4ff93674f9fedbed0597fb8e418a59b9ea70
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946562"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="4ed5f-103">Тип ресурса Иосбукмарк</span><span class="sxs-lookup"><span data-stu-id="4ed5f-103">iosBookmark resource type</span></span>

> <span data-ttu-id="4ed5f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ed5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ed5f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ed5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed5f-106">Закладка URL-адреса iOS</span><span class="sxs-lookup"><span data-stu-id="4ed5f-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="4ed5f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ed5f-107">Properties</span></span>
|<span data-ttu-id="4ed5f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ed5f-108">Property</span></span>|<span data-ttu-id="4ed5f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ed5f-109">Type</span></span>|<span data-ttu-id="4ed5f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ed5f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed5f-111">url</span><span class="sxs-lookup"><span data-stu-id="4ed5f-111">url</span></span>|<span data-ttu-id="4ed5f-112">String</span><span class="sxs-lookup"><span data-stu-id="4ed5f-112">String</span></span>|<span data-ttu-id="4ed5f-113">URL-адрес, разрешенный для доступа</span><span class="sxs-lookup"><span data-stu-id="4ed5f-113">URL allowed to access</span></span>|
|<span data-ttu-id="4ed5f-114">Букмаркфолдер</span><span class="sxs-lookup"><span data-stu-id="4ed5f-114">bookmarkFolder</span></span>|<span data-ttu-id="4ed5f-115">Строка</span><span class="sxs-lookup"><span data-stu-id="4ed5f-115">String</span></span>|<span data-ttu-id="4ed5f-116">Папка, в которую следует добавить закладку в Safari</span><span class="sxs-lookup"><span data-stu-id="4ed5f-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="4ed5f-117">displayName</span><span class="sxs-lookup"><span data-stu-id="4ed5f-117">displayName</span></span>|<span data-ttu-id="4ed5f-118">Строка</span><span class="sxs-lookup"><span data-stu-id="4ed5f-118">String</span></span>|<span data-ttu-id="4ed5f-119">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="4ed5f-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ed5f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4ed5f-120">Relationships</span></span>
<span data-ttu-id="4ed5f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4ed5f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ed5f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ed5f-122">JSON Representation</span></span>
<span data-ttu-id="4ed5f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ed5f-123">Here is a JSON representation of the resource.</span></span>
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




