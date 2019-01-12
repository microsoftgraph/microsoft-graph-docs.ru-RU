---
title: Тип ресурса iosBookmark
description: URL-адрес закладку операций ввода-вывода
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbf39a2eee5064b7d3ddfa474b1f70758d4c7047
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938176"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="502c9-103">Тип ресурса iosBookmark</span><span class="sxs-lookup"><span data-stu-id="502c9-103">iosBookmark resource type</span></span>

> <span data-ttu-id="502c9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="502c9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="502c9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="502c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="502c9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="502c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="502c9-107">URL-адрес закладку операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="502c9-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="502c9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="502c9-108">Properties</span></span>
|<span data-ttu-id="502c9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="502c9-109">Property</span></span>|<span data-ttu-id="502c9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="502c9-110">Type</span></span>|<span data-ttu-id="502c9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="502c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="502c9-112">url</span><span class="sxs-lookup"><span data-stu-id="502c9-112">url</span></span>|<span data-ttu-id="502c9-113">String</span><span class="sxs-lookup"><span data-stu-id="502c9-113">String</span></span>|<span data-ttu-id="502c9-114">Разрешен доступ к URL-адрес</span><span class="sxs-lookup"><span data-stu-id="502c9-114">URL allowed to access</span></span>|
|<span data-ttu-id="502c9-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="502c9-115">bookmarkFolder</span></span>|<span data-ttu-id="502c9-116">Строка</span><span class="sxs-lookup"><span data-stu-id="502c9-116">String</span></span>|<span data-ttu-id="502c9-117">Папка, в которую будет добавлен закладки в Safari</span><span class="sxs-lookup"><span data-stu-id="502c9-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="502c9-118">displayName</span><span class="sxs-lookup"><span data-stu-id="502c9-118">displayName</span></span>|<span data-ttu-id="502c9-119">Строка</span><span class="sxs-lookup"><span data-stu-id="502c9-119">String</span></span>|<span data-ttu-id="502c9-120">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="502c9-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="502c9-121">Связи</span><span class="sxs-lookup"><span data-stu-id="502c9-121">Relationships</span></span>
<span data-ttu-id="502c9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="502c9-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="502c9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="502c9-123">JSON Representation</span></span>
<span data-ttu-id="502c9-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="502c9-124">Here is a JSON representation of the resource.</span></span>
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





