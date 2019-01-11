---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5bcfc7f44399de72c27a631eb0d0f04ab76bd6a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813862"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="8b548-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="8b548-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="8b548-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b548-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b548-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b548-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b548-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8b548-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b548-107">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="8b548-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="8b548-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b548-108">Properties</span></span>
|<span data-ttu-id="8b548-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b548-109">Property</span></span>|<span data-ttu-id="8b548-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8b548-110">Type</span></span>|<span data-ttu-id="8b548-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8b548-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b548-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8b548-112">displayName</span></span>|<span data-ttu-id="8b548-113">String</span><span class="sxs-lookup"><span data-stu-id="8b548-113">String</span></span>|<span data-ttu-id="8b548-114">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="8b548-114">Name of the folder page</span></span>|
|<span data-ttu-id="8b548-115">apps</span><span class="sxs-lookup"><span data-stu-id="8b548-115">apps</span></span>|<span data-ttu-id="8b548-116">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b548-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="8b548-117">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="8b548-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="8b548-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8b548-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b548-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8b548-119">Relationships</span></span>
<span data-ttu-id="8b548-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8b548-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b548-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b548-121">JSON Representation</span></span>
<span data-ttu-id="8b548-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b548-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```





