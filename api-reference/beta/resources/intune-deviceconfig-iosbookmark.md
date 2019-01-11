---
title: Тип ресурса iosBookmark
description: URL-адрес закладку операций ввода-вывода
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 37cdcc1b886914b4b42e0a97e8947a565c75f5b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841001"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="a3f21-103">Тип ресурса iosBookmark</span><span class="sxs-lookup"><span data-stu-id="a3f21-103">iosBookmark resource type</span></span>

> <span data-ttu-id="a3f21-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3f21-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3f21-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3f21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3f21-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3f21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3f21-107">URL-адрес закладку операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="a3f21-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="a3f21-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3f21-108">Properties</span></span>
|<span data-ttu-id="a3f21-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3f21-109">Property</span></span>|<span data-ttu-id="a3f21-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a3f21-110">Type</span></span>|<span data-ttu-id="a3f21-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a3f21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3f21-112">url</span><span class="sxs-lookup"><span data-stu-id="a3f21-112">url</span></span>|<span data-ttu-id="a3f21-113">String</span><span class="sxs-lookup"><span data-stu-id="a3f21-113">String</span></span>|<span data-ttu-id="a3f21-114">Разрешен доступ к URL-адрес</span><span class="sxs-lookup"><span data-stu-id="a3f21-114">URL allowed to access</span></span>|
|<span data-ttu-id="a3f21-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="a3f21-115">bookmarkFolder</span></span>|<span data-ttu-id="a3f21-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a3f21-116">String</span></span>|<span data-ttu-id="a3f21-117">Папка, в которую будет добавлен закладки в Safari</span><span class="sxs-lookup"><span data-stu-id="a3f21-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="a3f21-118">displayName</span><span class="sxs-lookup"><span data-stu-id="a3f21-118">displayName</span></span>|<span data-ttu-id="a3f21-119">Строка</span><span class="sxs-lookup"><span data-stu-id="a3f21-119">String</span></span>|<span data-ttu-id="a3f21-120">Отображаемое имя закладки</span><span class="sxs-lookup"><span data-stu-id="a3f21-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3f21-121">Связи</span><span class="sxs-lookup"><span data-stu-id="a3f21-121">Relationships</span></span>
<span data-ttu-id="a3f21-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a3f21-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a3f21-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3f21-123">JSON Representation</span></span>
<span data-ttu-id="a3f21-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3f21-124">Here is a JSON representation of the resource.</span></span>
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





