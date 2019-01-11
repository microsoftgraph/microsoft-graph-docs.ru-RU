---
title: Тип ресурса iosWebContentFilterSpecificWebsitesAccess
description: Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который устанавливает закладки URL-адрес в браузере встроенных операций ввода-вывода. Пример сценария находится в классе, где преподавателей, предоставляемых студентов переходить веб-сайтов через браузер закладки, настроенного в своих устройствах iOS и нет доступа на другие сайты.
localization_priority: Normal
ms.openlocfilehash: 0dc3023c37311dc5fdeb2700b8a0fec58bdb4725
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844956"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="c8bd5-104">Тип ресурса iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="c8bd5-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="c8bd5-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8bd5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8bd5-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8bd5-108">Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который устанавливает закладки URL-адрес в браузере встроенных операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="c8bd5-109">Пример сценария находится в классе, где преподавателей, предоставляемых студентов переходить веб-сайтов через браузер закладки, настроенного в своих устройствах iOS и нет доступа на другие сайты.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>

<span data-ttu-id="c8bd5-110">Наследуется от [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="c8bd5-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8bd5-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8bd5-111">Properties</span></span>
|<span data-ttu-id="c8bd5-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8bd5-112">Property</span></span>|<span data-ttu-id="c8bd5-113">Тип</span><span class="sxs-lookup"><span data-stu-id="c8bd5-113">Type</span></span>|<span data-ttu-id="c8bd5-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c8bd5-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8bd5-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="c8bd5-115">specificWebsitesOnly</span></span>|<span data-ttu-id="c8bd5-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c8bd5-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="c8bd5-117">URL-адрес закладки, установленные в встроенных браузера и пользователей можно использовать только для доступа к веб-сайтов через закладки.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="c8bd5-118">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c8bd5-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="c8bd5-119">websiteList</span></span>|<span data-ttu-id="c8bd5-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c8bd5-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="c8bd5-121">URL-адрес закладки, установленные в встроенных браузера и пользователей можно использовать только для доступа к веб-сайтов через закладки.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="c8bd5-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8bd5-123">Связи</span><span class="sxs-lookup"><span data-stu-id="c8bd5-123">Relationships</span></span>
<span data-ttu-id="c8bd5-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c8bd5-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8bd5-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8bd5-125">JSON Representation</span></span>
<span data-ttu-id="c8bd5-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8bd5-126">Here is a JSON representation of the resource.</span></span>
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





