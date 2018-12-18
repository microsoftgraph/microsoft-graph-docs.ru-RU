---
title: Тип ресурса iosBookmark
description: URL-адрес закладку операций ввода-вывода
author: tfitzmac
ms.openlocfilehash: e1577537e57365b2452e956e010f6c3f918bd743
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308402"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="a7745-103">Тип ресурса iosBookmark</span><span class="sxs-lookup"><span data-stu-id="a7745-103">iosBookmark resource type</span></span>

> <span data-ttu-id="a7745-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a7745-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7745-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7745-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7745-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a7745-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7745-107">URL-адрес закладку операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="a7745-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="a7745-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7745-108">Properties</span></span>
|<span data-ttu-id="a7745-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7745-109">Property</span></span>|<span data-ttu-id="a7745-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a7745-110">Type</span></span>|<span data-ttu-id="a7745-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a7745-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7745-112">url</span><span class="sxs-lookup"><span data-stu-id="a7745-112">url</span></span>|<span data-ttu-id="a7745-113">String</span><span class="sxs-lookup"><span data-stu-id="a7745-113">String</span></span>|<span data-ttu-id="a7745-114">Разрешен доступ к URL-адрес</span><span class="sxs-lookup"><span data-stu-id="a7745-114">URL allowed to access</span></span>|
|<span data-ttu-id="a7745-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="a7745-115">bookmarkFolder</span></span>|<span data-ttu-id="a7745-116">String.</span><span class="sxs-lookup"><span data-stu-id="a7745-116">String</span></span>|<span data-ttu-id="a7745-117">Папка, в которую будет добавлен закладки в Safari</span><span class="sxs-lookup"><span data-stu-id="a7745-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="a7745-118">displayName</span><span class="sxs-lookup"><span data-stu-id="a7745-118">displayName</span></span>|<span data-ttu-id="a7745-119">Строка</span><span class="sxs-lookup"><span data-stu-id="a7745-119">String</span></span>|<span data-ttu-id="a7745-120">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="a7745-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7745-121">Связи</span><span class="sxs-lookup"><span data-stu-id="a7745-121">Relationships</span></span>
<span data-ttu-id="a7745-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a7745-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a7745-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7745-123">JSON Representation</span></span>
<span data-ttu-id="a7745-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7745-124">Here is a JSON representation of the resource.</span></span>
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





