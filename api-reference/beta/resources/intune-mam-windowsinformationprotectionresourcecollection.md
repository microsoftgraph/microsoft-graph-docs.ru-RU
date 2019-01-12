---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a65704170c048f4aae66876f11ef8543c7b09e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933010"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="fa5aa-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="fa5aa-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="fa5aa-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa5aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa5aa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa5aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa5aa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa5aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa5aa-107">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fa5aa-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="fa5aa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa5aa-108">Properties</span></span>
|<span data-ttu-id="fa5aa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa5aa-109">Property</span></span>|<span data-ttu-id="fa5aa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fa5aa-110">Type</span></span>|<span data-ttu-id="fa5aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa5aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa5aa-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fa5aa-112">displayName</span></span>|<span data-ttu-id="fa5aa-113">Строка</span><span class="sxs-lookup"><span data-stu-id="fa5aa-113">String</span></span>|<span data-ttu-id="fa5aa-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="fa5aa-114">Display name</span></span>|
|<span data-ttu-id="fa5aa-115">resources</span><span class="sxs-lookup"><span data-stu-id="fa5aa-115">resources</span></span>|<span data-ttu-id="fa5aa-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fa5aa-116">String collection</span></span>|<span data-ttu-id="fa5aa-117">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="fa5aa-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa5aa-118">Связи</span><span class="sxs-lookup"><span data-stu-id="fa5aa-118">Relationships</span></span>
<span data-ttu-id="fa5aa-119">Нет</span><span class="sxs-lookup"><span data-stu-id="fa5aa-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa5aa-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa5aa-120">JSON Representation</span></span>
<span data-ttu-id="fa5aa-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa5aa-121">Here is a JSON representation of the resource.</span></span>
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





