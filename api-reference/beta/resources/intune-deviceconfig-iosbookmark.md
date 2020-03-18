---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 465aafff3910eb0d62990a14a42ce4cb79a16334
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791690"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="f2358-103">Тип ресурса Иосбукмарк</span><span class="sxs-lookup"><span data-stu-id="f2358-103">iosBookmark resource type</span></span>

> <span data-ttu-id="f2358-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2358-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2358-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2358-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2358-106">Закладка URL-адреса iOS</span><span class="sxs-lookup"><span data-stu-id="f2358-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="f2358-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2358-107">Properties</span></span>
|<span data-ttu-id="f2358-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2358-108">Property</span></span>|<span data-ttu-id="f2358-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f2358-109">Type</span></span>|<span data-ttu-id="f2358-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f2358-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2358-111">url</span><span class="sxs-lookup"><span data-stu-id="f2358-111">url</span></span>|<span data-ttu-id="f2358-112">String</span><span class="sxs-lookup"><span data-stu-id="f2358-112">String</span></span>|<span data-ttu-id="f2358-113">URL-адрес, разрешенный для доступа</span><span class="sxs-lookup"><span data-stu-id="f2358-113">URL allowed to access</span></span>|
|<span data-ttu-id="f2358-114">букмаркфолдер</span><span class="sxs-lookup"><span data-stu-id="f2358-114">bookmarkFolder</span></span>|<span data-ttu-id="f2358-115">String</span><span class="sxs-lookup"><span data-stu-id="f2358-115">String</span></span>|<span data-ttu-id="f2358-116">Папка, в которую следует добавить закладку в Safari</span><span class="sxs-lookup"><span data-stu-id="f2358-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="f2358-117">displayName</span><span class="sxs-lookup"><span data-stu-id="f2358-117">displayName</span></span>|<span data-ttu-id="f2358-118">String</span><span class="sxs-lookup"><span data-stu-id="f2358-118">String</span></span>|<span data-ttu-id="f2358-119">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="f2358-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2358-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f2358-120">Relationships</span></span>
<span data-ttu-id="f2358-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f2358-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2358-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2358-122">JSON Representation</span></span>
<span data-ttu-id="f2358-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2358-123">Here is a JSON representation of the resource.</span></span>
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



