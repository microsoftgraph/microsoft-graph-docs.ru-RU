---
title: Тип ресурса ИосвебконтентфилтерспеЦификвебситесакцесс
description: Представляет тип параметра фильтра веб-содержимого iOS, который устанавливает закладки URL-адресов в встроенный браузер iOS. Пример сценария — это аудитория, в которой преподаватели хотели бы перемещаться по веб-сайтам с помощью закладок браузера, настроенных на устройствах iOS, и без доступа к другим сайтам.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa2e0ee1a699c4058bfd246efc45d05516bca460
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985334"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="1ddd7-104">Тип ресурса ИосвебконтентфилтерспеЦификвебситесакцесс</span><span class="sxs-lookup"><span data-stu-id="1ddd7-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="1ddd7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ddd7-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ddd7-107">Представляет тип параметра фильтра веб-содержимого iOS, который устанавливает закладки URL-адресов в встроенный браузер iOS.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-107">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="1ddd7-108">Пример сценария — это аудитория, в которой преподаватели хотели бы перемещаться по веб-сайтам с помощью закладок браузера, настроенных на устройствах iOS, и без доступа к другим сайтам.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-108">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="1ddd7-109">Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="1ddd7-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ddd7-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ddd7-110">Properties</span></span>
|<span data-ttu-id="1ddd7-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ddd7-111">Property</span></span>|<span data-ttu-id="1ddd7-112">Тип</span><span class="sxs-lookup"><span data-stu-id="1ddd7-112">Type</span></span>|<span data-ttu-id="1ddd7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1ddd7-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ddd7-114">СпеЦификвебситесонли</span><span class="sxs-lookup"><span data-stu-id="1ddd7-114">specificWebsitesOnly</span></span>|<span data-ttu-id="1ddd7-115">Коллекция [иосбукмарк](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="1ddd7-115">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="1ddd7-116">Закладки URL-адресов, которые будут установлены во встроенный браузер, и пользователи могут получать доступ к веб-сайтам только с помощью закладок.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-116">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="1ddd7-117">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-117">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1ddd7-118">Вебсителист</span><span class="sxs-lookup"><span data-stu-id="1ddd7-118">websiteList</span></span>|<span data-ttu-id="1ddd7-119">Коллекция [иосбукмарк](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="1ddd7-119">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="1ddd7-120">Закладки URL-адресов, которые будут установлены во встроенный браузер, и пользователи могут получать доступ к веб-сайтам только с помощью закладок.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-120">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="1ddd7-121">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ddd7-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ddd7-122">Relationships</span></span>
<span data-ttu-id="1ddd7-123">Нет</span><span class="sxs-lookup"><span data-stu-id="1ddd7-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ddd7-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ddd7-124">JSON Representation</span></span>
<span data-ttu-id="1ddd7-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ddd7-125">Here is a JSON representation of the resource.</span></span>
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





