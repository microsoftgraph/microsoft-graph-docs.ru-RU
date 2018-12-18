---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: tfitzmac
ms.openlocfilehash: 96b3b36f40d1eeb88731f6f44ebec812a18fe713
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306890"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="2f7dc-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="2f7dc-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="2f7dc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f7dc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f7dc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f7dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f7dc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f7dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f7dc-107">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="2f7dc-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="2f7dc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f7dc-108">Properties</span></span>
|<span data-ttu-id="2f7dc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f7dc-109">Property</span></span>|<span data-ttu-id="2f7dc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2f7dc-110">Type</span></span>|<span data-ttu-id="2f7dc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2f7dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f7dc-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2f7dc-112">displayName</span></span>|<span data-ttu-id="2f7dc-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2f7dc-113">String</span></span>|<span data-ttu-id="2f7dc-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="2f7dc-114">Display name</span></span>|
|<span data-ttu-id="2f7dc-115">resources</span><span class="sxs-lookup"><span data-stu-id="2f7dc-115">resources</span></span>|<span data-ttu-id="2f7dc-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2f7dc-116">String collection</span></span>|<span data-ttu-id="2f7dc-117">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="2f7dc-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f7dc-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2f7dc-118">Relationships</span></span>
<span data-ttu-id="2f7dc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2f7dc-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2f7dc-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f7dc-120">JSON Representation</span></span>
<span data-ttu-id="2f7dc-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f7dc-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```





