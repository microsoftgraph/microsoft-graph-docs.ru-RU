---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7cde9f58fd7deb66fb30f871d1ff7d0968835a40
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795928"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="1a47c-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="1a47c-103">appListItem resource type</span></span>

> <span data-ttu-id="1a47c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a47c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a47c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a47c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a47c-106">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="1a47c-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="1a47c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a47c-107">Properties</span></span>
|<span data-ttu-id="1a47c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a47c-108">Property</span></span>|<span data-ttu-id="1a47c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1a47c-109">Type</span></span>|<span data-ttu-id="1a47c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a47c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a47c-111">name</span><span class="sxs-lookup"><span data-stu-id="1a47c-111">name</span></span>|<span data-ttu-id="1a47c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="1a47c-112">String</span></span>|<span data-ttu-id="1a47c-113">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="1a47c-113">The application name</span></span>|
|<span data-ttu-id="1a47c-114">publisher</span><span class="sxs-lookup"><span data-stu-id="1a47c-114">publisher</span></span>|<span data-ttu-id="1a47c-115">String</span><span class="sxs-lookup"><span data-stu-id="1a47c-115">String</span></span>|<span data-ttu-id="1a47c-116">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="1a47c-116">The publisher of the application</span></span>|
|<span data-ttu-id="1a47c-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1a47c-117">appStoreUrl</span></span>|<span data-ttu-id="1a47c-118">String</span><span class="sxs-lookup"><span data-stu-id="1a47c-118">String</span></span>|<span data-ttu-id="1a47c-119">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="1a47c-119">The Store URL of the application</span></span>|
|<span data-ttu-id="1a47c-120">appId</span><span class="sxs-lookup"><span data-stu-id="1a47c-120">appId</span></span>|<span data-ttu-id="1a47c-121">String</span><span class="sxs-lookup"><span data-stu-id="1a47c-121">String</span></span>|<span data-ttu-id="1a47c-122">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="1a47c-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a47c-123">Связи</span><span class="sxs-lookup"><span data-stu-id="1a47c-123">Relationships</span></span>
<span data-ttu-id="1a47c-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1a47c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a47c-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a47c-125">JSON Representation</span></span>
<span data-ttu-id="1a47c-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a47c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



