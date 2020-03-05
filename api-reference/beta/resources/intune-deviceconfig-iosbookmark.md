---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a297dcf731f1bec513f25896c3025e337358b85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529958"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="d90bf-103">Тип ресурса Иосбукмарк</span><span class="sxs-lookup"><span data-stu-id="d90bf-103">iosBookmark resource type</span></span>

<span data-ttu-id="d90bf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d90bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d90bf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d90bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d90bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d90bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d90bf-107">Закладка URL-адреса iOS</span><span class="sxs-lookup"><span data-stu-id="d90bf-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="d90bf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d90bf-108">Properties</span></span>
|<span data-ttu-id="d90bf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d90bf-109">Property</span></span>|<span data-ttu-id="d90bf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d90bf-110">Type</span></span>|<span data-ttu-id="d90bf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d90bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d90bf-112">url</span><span class="sxs-lookup"><span data-stu-id="d90bf-112">url</span></span>|<span data-ttu-id="d90bf-113">String</span><span class="sxs-lookup"><span data-stu-id="d90bf-113">String</span></span>|<span data-ttu-id="d90bf-114">URL-адрес, разрешенный для доступа</span><span class="sxs-lookup"><span data-stu-id="d90bf-114">URL allowed to access</span></span>|
|<span data-ttu-id="d90bf-115">букмаркфолдер</span><span class="sxs-lookup"><span data-stu-id="d90bf-115">bookmarkFolder</span></span>|<span data-ttu-id="d90bf-116">String</span><span class="sxs-lookup"><span data-stu-id="d90bf-116">String</span></span>|<span data-ttu-id="d90bf-117">Папка, в которую следует добавить закладку в Safari</span><span class="sxs-lookup"><span data-stu-id="d90bf-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="d90bf-118">displayName</span><span class="sxs-lookup"><span data-stu-id="d90bf-118">displayName</span></span>|<span data-ttu-id="d90bf-119">String</span><span class="sxs-lookup"><span data-stu-id="d90bf-119">String</span></span>|<span data-ttu-id="d90bf-120">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="d90bf-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="d90bf-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d90bf-121">Relationships</span></span>
<span data-ttu-id="d90bf-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d90bf-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d90bf-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d90bf-123">JSON Representation</span></span>
<span data-ttu-id="d90bf-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d90bf-124">Here is a JSON representation of the resource.</span></span>
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



