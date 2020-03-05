---
title: Тип ресурса ИосвебконтентфилтерспеЦификвебситесакцесс
description: Представляет тип параметра фильтра веб-содержимого iOS, который устанавливает закладки URL-адресов в встроенный браузер iOS. Пример сценария — это аудитория, в которой преподаватели хотели бы перемещаться по веб-сайтам с помощью закладок браузера, настроенных на устройствах iOS, и без доступа к другим сайтам.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4129ce4f4332c78e5af6170b5ce48ab7aa19cee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529809"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="1d5a1-104">Тип ресурса ИосвебконтентфилтерспеЦификвебситесакцесс</span><span class="sxs-lookup"><span data-stu-id="1d5a1-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

<span data-ttu-id="1d5a1-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1d5a1-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d5a1-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d5a1-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d5a1-108">Представляет тип параметра фильтра веб-содержимого iOS, который устанавливает закладки URL-адресов в встроенный браузер iOS.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="1d5a1-109">Пример сценария — это аудитория, в которой преподаватели хотели бы перемещаться по веб-сайтам с помощью закладок браузера, настроенных на устройствах iOS, и без доступа к другим сайтам.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="1d5a1-110">Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="1d5a1-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1d5a1-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d5a1-111">Properties</span></span>
|<span data-ttu-id="1d5a1-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d5a1-112">Property</span></span>|<span data-ttu-id="1d5a1-113">Тип</span><span class="sxs-lookup"><span data-stu-id="1d5a1-113">Type</span></span>|<span data-ttu-id="1d5a1-114">Описание</span><span class="sxs-lookup"><span data-stu-id="1d5a1-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d5a1-115">спеЦификвебситесонли</span><span class="sxs-lookup"><span data-stu-id="1d5a1-115">specificWebsitesOnly</span></span>|<span data-ttu-id="1d5a1-116">Коллекция [иосбукмарк](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="1d5a1-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="1d5a1-117">Закладки URL-адресов, которые будут установлены во встроенный браузер, и пользователи могут получать доступ к веб-сайтам только с помощью закладок.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="1d5a1-118">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1d5a1-119">вебсителист</span><span class="sxs-lookup"><span data-stu-id="1d5a1-119">websiteList</span></span>|<span data-ttu-id="1d5a1-120">Коллекция [иосбукмарк](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="1d5a1-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="1d5a1-121">Закладки URL-адресов, которые будут установлены во встроенный браузер, и пользователи могут получать доступ к веб-сайтам только с помощью закладок.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="1d5a1-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d5a1-123">Связи</span><span class="sxs-lookup"><span data-stu-id="1d5a1-123">Relationships</span></span>
<span data-ttu-id="1d5a1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1d5a1-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d5a1-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d5a1-125">JSON Representation</span></span>
<span data-ttu-id="1d5a1-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d5a1-126">Here is a JSON representation of the resource.</span></span>
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



