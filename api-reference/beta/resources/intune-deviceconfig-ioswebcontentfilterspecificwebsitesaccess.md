---
title: Тип ресурса iosWebContentFilterSpecificWebsitesAccess
description: Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который устанавливает закладки URL-адрес в браузере встроенных операций ввода-вывода. Пример сценария находится в классе, где преподавателей, предоставляемых студентов переходить веб-сайтов через браузер закладки, настроенного в своих устройствах iOS и нет доступа на другие сайты.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 964ade2d2b46755fbba2903c6e9607340f60aedf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424765"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="ba974-104">Тип ресурса iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="ba974-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="ba974-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba974-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ba974-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba974-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba974-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba974-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba974-108">Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который устанавливает закладки URL-адрес в браузере встроенных операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="ba974-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="ba974-109">Пример сценария находится в классе, где преподавателей, предоставляемых студентов переходить веб-сайтов через браузер закладки, настроенного в своих устройствах iOS и нет доступа на другие сайты.</span><span class="sxs-lookup"><span data-stu-id="ba974-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="ba974-110">Наследуется от [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="ba974-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ba974-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba974-111">Properties</span></span>
|<span data-ttu-id="ba974-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba974-112">Property</span></span>|<span data-ttu-id="ba974-113">Тип</span><span class="sxs-lookup"><span data-stu-id="ba974-113">Type</span></span>|<span data-ttu-id="ba974-114">Описание</span><span class="sxs-lookup"><span data-stu-id="ba974-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba974-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="ba974-115">specificWebsitesOnly</span></span>|<span data-ttu-id="ba974-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ba974-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="ba974-117">URL-адрес закладки, установленные в встроенных браузера и пользователей можно использовать только для доступа к веб-сайтов через закладки.</span><span class="sxs-lookup"><span data-stu-id="ba974-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="ba974-118">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ba974-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ba974-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="ba974-119">websiteList</span></span>|<span data-ttu-id="ba974-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ba974-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="ba974-121">URL-адрес закладки, установленные в встроенных браузера и пользователей можно использовать только для доступа к веб-сайтов через закладки.</span><span class="sxs-lookup"><span data-stu-id="ba974-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="ba974-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ba974-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba974-123">Связи</span><span class="sxs-lookup"><span data-stu-id="ba974-123">Relationships</span></span>
<span data-ttu-id="ba974-124">Нет</span><span class="sxs-lookup"><span data-stu-id="ba974-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba974-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba974-125">JSON Representation</span></span>
<span data-ttu-id="ba974-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba974-126">Here is a JSON representation of the resource.</span></span>
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




