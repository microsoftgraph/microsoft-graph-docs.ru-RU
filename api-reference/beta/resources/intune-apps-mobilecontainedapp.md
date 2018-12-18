---
title: Тип ресурса mobileContainedApp
description: Абстрактный класс, представляющий автономные приложения в mobileApp, работающие в качестве пакета.
author: tfitzmac
ms.openlocfilehash: 314225c46247bd122c825f0f883378513445ce0a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340798"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="311db-103">Тип ресурса mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="311db-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="311db-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="311db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="311db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="311db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="311db-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="311db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="311db-107">Абстрактный класс, представляющий автономные приложения в mobileApp, работающие в качестве пакета.</span><span class="sxs-lookup"><span data-stu-id="311db-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>
## <a name="methods"></a><span data-ttu-id="311db-108">Методы</span><span class="sxs-lookup"><span data-stu-id="311db-108">Methods</span></span>
|<span data-ttu-id="311db-109">Метод</span><span class="sxs-lookup"><span data-stu-id="311db-109">Method</span></span>|<span data-ttu-id="311db-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="311db-110">Return Type</span></span>|<span data-ttu-id="311db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="311db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="311db-112">Список mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="311db-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="311db-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="311db-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="311db-114">Свойства списка и связей объектов [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="311db-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="311db-115">Получение mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="311db-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|<span data-ttu-id="311db-116">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md);</span><span class="sxs-lookup"><span data-stu-id="311db-116">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|<span data-ttu-id="311db-117">Чтение свойства и связи объекта [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="311db-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="311db-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="311db-118">Properties</span></span>
|<span data-ttu-id="311db-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="311db-119">Property</span></span>|<span data-ttu-id="311db-120">Тип</span><span class="sxs-lookup"><span data-stu-id="311db-120">Type</span></span>|<span data-ttu-id="311db-121">Описание</span><span class="sxs-lookup"><span data-stu-id="311db-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="311db-122">id</span><span class="sxs-lookup"><span data-stu-id="311db-122">id</span></span>|<span data-ttu-id="311db-123">Строка</span><span class="sxs-lookup"><span data-stu-id="311db-123">String</span></span>|<span data-ttu-id="311db-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="311db-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="311db-125">Связи</span><span class="sxs-lookup"><span data-stu-id="311db-125">Relationships</span></span>
<span data-ttu-id="311db-126">Нет</span><span class="sxs-lookup"><span data-stu-id="311db-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="311db-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="311db-127">JSON Representation</span></span>
<span data-ttu-id="311db-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="311db-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```





