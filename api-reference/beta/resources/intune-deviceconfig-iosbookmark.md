---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7bfc889acd17049e38a0e4efe03d83389e9983fd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729697"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="8ea5d-103">Тип ресурса Иосбукмарк</span><span class="sxs-lookup"><span data-stu-id="8ea5d-103">iosBookmark resource type</span></span>

<span data-ttu-id="8ea5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ea5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ea5d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ea5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ea5d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ea5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ea5d-107">Закладка URL-адреса iOS</span><span class="sxs-lookup"><span data-stu-id="8ea5d-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="8ea5d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ea5d-108">Properties</span></span>
|<span data-ttu-id="8ea5d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ea5d-109">Property</span></span>|<span data-ttu-id="8ea5d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8ea5d-110">Type</span></span>|<span data-ttu-id="8ea5d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ea5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ea5d-112">url</span><span class="sxs-lookup"><span data-stu-id="8ea5d-112">url</span></span>|<span data-ttu-id="8ea5d-113">String</span><span class="sxs-lookup"><span data-stu-id="8ea5d-113">String</span></span>|<span data-ttu-id="8ea5d-114">URL-адрес, разрешенный для доступа</span><span class="sxs-lookup"><span data-stu-id="8ea5d-114">URL allowed to access</span></span>|
|<span data-ttu-id="8ea5d-115">букмаркфолдер</span><span class="sxs-lookup"><span data-stu-id="8ea5d-115">bookmarkFolder</span></span>|<span data-ttu-id="8ea5d-116">Строка</span><span class="sxs-lookup"><span data-stu-id="8ea5d-116">String</span></span>|<span data-ttu-id="8ea5d-117">Папка, в которую следует добавить закладку в Safari</span><span class="sxs-lookup"><span data-stu-id="8ea5d-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="8ea5d-118">displayName</span><span class="sxs-lookup"><span data-stu-id="8ea5d-118">displayName</span></span>|<span data-ttu-id="8ea5d-119">Строка</span><span class="sxs-lookup"><span data-stu-id="8ea5d-119">String</span></span>|<span data-ttu-id="8ea5d-120">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="8ea5d-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ea5d-121">Связи</span><span class="sxs-lookup"><span data-stu-id="8ea5d-121">Relationships</span></span>
<span data-ttu-id="8ea5d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8ea5d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ea5d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ea5d-123">JSON Representation</span></span>
<span data-ttu-id="8ea5d-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ea5d-124">Here is a JSON representation of the resource.</span></span>
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





