---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
ms.openlocfilehash: ac43ddbd18e99983bf4d06e9ceb97445b9d4bf57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081570"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="b81a6-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="b81a6-103">keyValuePair resource type</span></span>

> <span data-ttu-id="b81a6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b81a6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b81a6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b81a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b81a6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b81a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b81a6-107">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="b81a6-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="b81a6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b81a6-108">Properties</span></span>
|<span data-ttu-id="b81a6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b81a6-109">Property</span></span>|<span data-ttu-id="b81a6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b81a6-110">Type</span></span>|<span data-ttu-id="b81a6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b81a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b81a6-112">name</span><span class="sxs-lookup"><span data-stu-id="b81a6-112">name</span></span>|<span data-ttu-id="b81a6-113">String</span><span class="sxs-lookup"><span data-stu-id="b81a6-113">String</span></span>|<span data-ttu-id="b81a6-114">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="b81a6-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="b81a6-115">value</span><span class="sxs-lookup"><span data-stu-id="b81a6-115">value</span></span>|<span data-ttu-id="b81a6-116">String</span><span class="sxs-lookup"><span data-stu-id="b81a6-116">String</span></span>|<span data-ttu-id="b81a6-117">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="b81a6-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="b81a6-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b81a6-118">Relationships</span></span>
<span data-ttu-id="b81a6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b81a6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b81a6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b81a6-120">JSON Representation</span></span>
<span data-ttu-id="b81a6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b81a6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```





