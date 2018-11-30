---
title: Тип ресурса resourceAction
description: Н/Д
ms.openlocfilehash: 4cbfc149207f2f7589bd7e05075326641d4e8b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024491"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="8cef2-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="8cef2-103">resourceAction resource type</span></span>

> <span data-ttu-id="8cef2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8cef2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cef2-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8cef2-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8cef2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cef2-106">Properties</span></span>
|<span data-ttu-id="8cef2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cef2-107">Property</span></span>|<span data-ttu-id="8cef2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8cef2-108">Type</span></span>|<span data-ttu-id="8cef2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8cef2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cef2-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="8cef2-110">allowedResourceActions</span></span>|<span data-ttu-id="8cef2-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8cef2-111">String collection</span></span>|<span data-ttu-id="8cef2-112">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="8cef2-112">Allowed Actions</span></span>|
|<span data-ttu-id="8cef2-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="8cef2-113">notAllowedResourceActions</span></span>|<span data-ttu-id="8cef2-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8cef2-114">String collection</span></span>|<span data-ttu-id="8cef2-115">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="8cef2-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cef2-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8cef2-116">Relationships</span></span>
<span data-ttu-id="8cef2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8cef2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8cef2-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cef2-118">JSON Representation</span></span>
<span data-ttu-id="8cef2-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cef2-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



