---
title: Тип ресурса ИосвебконтентфилтерспеЦификвебситесакцесс
description: Представляет тип параметра фильтра веб-содержимого iOS, который устанавливает закладки URL-адресов в встроенный браузер iOS. Пример сценария — это аудитория, в которой преподаватели хотели бы перемещаться по веб-сайтам с помощью закладок браузера, настроенных на устройствах iOS, и без доступа к другим сайтам.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f5cadbc1ba359f53fadd46fb575465e33546ba61
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092582"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="34e3f-104">Тип ресурса ИосвебконтентфилтерспеЦификвебситесакцесс</span><span class="sxs-lookup"><span data-stu-id="34e3f-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

<span data-ttu-id="34e3f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34e3f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34e3f-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34e3f-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34e3f-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34e3f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34e3f-108">Представляет тип параметра фильтра веб-содержимого iOS, который устанавливает закладки URL-адресов в встроенный браузер iOS.</span><span class="sxs-lookup"><span data-stu-id="34e3f-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="34e3f-109">Пример сценария — это аудитория, в которой преподаватели хотели бы перемещаться по веб-сайтам с помощью закладок браузера, настроенных на устройствах iOS, и без доступа к другим сайтам.</span><span class="sxs-lookup"><span data-stu-id="34e3f-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="34e3f-110">Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="34e3f-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34e3f-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="34e3f-111">Properties</span></span>
|<span data-ttu-id="34e3f-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="34e3f-112">Property</span></span>|<span data-ttu-id="34e3f-113">Тип</span><span class="sxs-lookup"><span data-stu-id="34e3f-113">Type</span></span>|<span data-ttu-id="34e3f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="34e3f-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34e3f-115">спеЦификвебситесонли</span><span class="sxs-lookup"><span data-stu-id="34e3f-115">specificWebsitesOnly</span></span>|<span data-ttu-id="34e3f-116">Коллекция [иосбукмарк](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="34e3f-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="34e3f-117">Закладки URL-адресов, которые будут установлены во встроенный браузер, и пользователи могут получать доступ к веб-сайтам только с помощью закладок.</span><span class="sxs-lookup"><span data-stu-id="34e3f-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="34e3f-118">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="34e3f-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="34e3f-119">вебсителист</span><span class="sxs-lookup"><span data-stu-id="34e3f-119">websiteList</span></span>|<span data-ttu-id="34e3f-120">Коллекция [иосбукмарк](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="34e3f-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="34e3f-121">Закладки URL-адресов, которые будут установлены во встроенный браузер, и пользователи могут получать доступ к веб-сайтам только с помощью закладок.</span><span class="sxs-lookup"><span data-stu-id="34e3f-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="34e3f-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="34e3f-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34e3f-123">Связи</span><span class="sxs-lookup"><span data-stu-id="34e3f-123">Relationships</span></span>
<span data-ttu-id="34e3f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="34e3f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34e3f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34e3f-125">JSON Representation</span></span>
<span data-ttu-id="34e3f-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34e3f-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```






