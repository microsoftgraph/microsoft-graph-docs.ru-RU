---
title: Тип ресурса Апплеапплиститем
description: Представляет приложение в списке управляемых приложений Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4804f3834a63a3c446c09d383c2244def97398
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470127"
---
# <a name="appleapplistitem-resource-type"></a><span data-ttu-id="411fa-103">Тип ресурса Апплеапплиститем</span><span class="sxs-lookup"><span data-stu-id="411fa-103">appleAppListItem resource type</span></span>

<span data-ttu-id="411fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="411fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="411fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="411fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="411fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="411fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="411fa-107">Представляет приложение в списке управляемых приложений Apple</span><span class="sxs-lookup"><span data-stu-id="411fa-107">Represents an app in the list of managed Apple applications</span></span>


<span data-ttu-id="411fa-108">Наследуется от [апплиститем](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="411fa-108">Inherits from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="411fa-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="411fa-109">Properties</span></span>
|<span data-ttu-id="411fa-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="411fa-110">Property</span></span>|<span data-ttu-id="411fa-111">Тип</span><span class="sxs-lookup"><span data-stu-id="411fa-111">Type</span></span>|<span data-ttu-id="411fa-112">Описание</span><span class="sxs-lookup"><span data-stu-id="411fa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="411fa-113">name</span><span class="sxs-lookup"><span data-stu-id="411fa-113">name</span></span>|<span data-ttu-id="411fa-114">Строка</span><span class="sxs-lookup"><span data-stu-id="411fa-114">String</span></span>|<span data-ttu-id="411fa-115">Имя приложения, унаследованное от [апплиститем](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="411fa-115">The application name Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="411fa-116">publisher</span><span class="sxs-lookup"><span data-stu-id="411fa-116">publisher</span></span>|<span data-ttu-id="411fa-117">String</span><span class="sxs-lookup"><span data-stu-id="411fa-117">String</span></span>|<span data-ttu-id="411fa-118">Издатель приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="411fa-118">The publisher of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="411fa-119">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="411fa-119">appStoreUrl</span></span>|<span data-ttu-id="411fa-120">String</span><span class="sxs-lookup"><span data-stu-id="411fa-120">String</span></span>|<span data-ttu-id="411fa-121">URL-адрес хранилища приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="411fa-121">The Store URL of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="411fa-122">appId</span><span class="sxs-lookup"><span data-stu-id="411fa-122">appId</span></span>|<span data-ttu-id="411fa-123">String</span><span class="sxs-lookup"><span data-stu-id="411fa-123">String</span></span>|<span data-ttu-id="411fa-124">Идентификатор пакета приложения, унаследованного от [апплиститем](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="411fa-124">The bundle identifier of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="411fa-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="411fa-125">Relationships</span></span>
<span data-ttu-id="411fa-126">Нет</span><span class="sxs-lookup"><span data-stu-id="411fa-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="411fa-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="411fa-127">JSON Representation</span></span>
<span data-ttu-id="411fa-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="411fa-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



