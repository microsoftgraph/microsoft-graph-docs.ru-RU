---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3789d905d285561e56b7a21664214f777987524e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444201"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="d4426-103">Тип ресурса Иосбукмарк</span><span class="sxs-lookup"><span data-stu-id="d4426-103">iosBookmark resource type</span></span>

<span data-ttu-id="d4426-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4426-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4426-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4426-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4426-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4426-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4426-107">Закладка URL-адреса iOS</span><span class="sxs-lookup"><span data-stu-id="d4426-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="d4426-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4426-108">Properties</span></span>
|<span data-ttu-id="d4426-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4426-109">Property</span></span>|<span data-ttu-id="d4426-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d4426-110">Type</span></span>|<span data-ttu-id="d4426-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d4426-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4426-112">url</span><span class="sxs-lookup"><span data-stu-id="d4426-112">url</span></span>|<span data-ttu-id="d4426-113">String</span><span class="sxs-lookup"><span data-stu-id="d4426-113">String</span></span>|<span data-ttu-id="d4426-114">URL-адрес, разрешенный для доступа</span><span class="sxs-lookup"><span data-stu-id="d4426-114">URL allowed to access</span></span>|
|<span data-ttu-id="d4426-115">букмаркфолдер</span><span class="sxs-lookup"><span data-stu-id="d4426-115">bookmarkFolder</span></span>|<span data-ttu-id="d4426-116">String</span><span class="sxs-lookup"><span data-stu-id="d4426-116">String</span></span>|<span data-ttu-id="d4426-117">Папка, в которую следует добавить закладку в Safari</span><span class="sxs-lookup"><span data-stu-id="d4426-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="d4426-118">displayName</span><span class="sxs-lookup"><span data-stu-id="d4426-118">displayName</span></span>|<span data-ttu-id="d4426-119">String</span><span class="sxs-lookup"><span data-stu-id="d4426-119">String</span></span>|<span data-ttu-id="d4426-120">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="d4426-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4426-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d4426-121">Relationships</span></span>
<span data-ttu-id="d4426-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d4426-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4426-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4426-123">JSON Representation</span></span>
<span data-ttu-id="d4426-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4426-124">Here is a JSON representation of the resource.</span></span>
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



