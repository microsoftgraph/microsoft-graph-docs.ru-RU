---
title: Тип ресурса iosBookmark
description: URL-адрес закладку операций ввода-вывода
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e95f3bfd40bdf5ca5782aa9233a020623d32d6a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395911"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="bd50d-103">Тип ресурса iosBookmark</span><span class="sxs-lookup"><span data-stu-id="bd50d-103">iosBookmark resource type</span></span>

> <span data-ttu-id="bd50d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd50d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd50d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd50d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd50d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd50d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd50d-107">URL-адрес закладку операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="bd50d-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="bd50d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd50d-108">Properties</span></span>
|<span data-ttu-id="bd50d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd50d-109">Property</span></span>|<span data-ttu-id="bd50d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bd50d-110">Type</span></span>|<span data-ttu-id="bd50d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd50d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd50d-112">url</span><span class="sxs-lookup"><span data-stu-id="bd50d-112">url</span></span>|<span data-ttu-id="bd50d-113">String</span><span class="sxs-lookup"><span data-stu-id="bd50d-113">String</span></span>|<span data-ttu-id="bd50d-114">Разрешен доступ к URL-адрес</span><span class="sxs-lookup"><span data-stu-id="bd50d-114">URL allowed to access</span></span>|
|<span data-ttu-id="bd50d-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="bd50d-115">bookmarkFolder</span></span>|<span data-ttu-id="bd50d-116">String</span><span class="sxs-lookup"><span data-stu-id="bd50d-116">String</span></span>|<span data-ttu-id="bd50d-117">Папка, в которую будет добавлен закладки в Safari</span><span class="sxs-lookup"><span data-stu-id="bd50d-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="bd50d-118">displayName</span><span class="sxs-lookup"><span data-stu-id="bd50d-118">displayName</span></span>|<span data-ttu-id="bd50d-119">String</span><span class="sxs-lookup"><span data-stu-id="bd50d-119">String</span></span>|<span data-ttu-id="bd50d-120">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="bd50d-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd50d-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="bd50d-121">Relationships</span></span>
<span data-ttu-id="bd50d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="bd50d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd50d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd50d-123">JSON Representation</span></span>
<span data-ttu-id="bd50d-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd50d-124">Here is a JSON representation of the resource.</span></span>
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




