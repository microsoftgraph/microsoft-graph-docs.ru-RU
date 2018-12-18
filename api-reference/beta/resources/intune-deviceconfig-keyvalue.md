---
title: Тип ресурса keyValue
description: Определение значения ключа.
author: tfitzmac
ms.openlocfilehash: 5e5754657e679f3a703c2b5dec7cea36d1bad860
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302641"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="30b70-103">Тип ресурса keyValue</span><span class="sxs-lookup"><span data-stu-id="30b70-103">keyValue resource type</span></span>

> <span data-ttu-id="30b70-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="30b70-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30b70-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30b70-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="30b70-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30b70-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="30b70-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="30b70-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="30b70-108">Properties</span></span>
|<span data-ttu-id="30b70-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="30b70-109">Property</span></span>|<span data-ttu-id="30b70-110">Тип</span><span class="sxs-lookup"><span data-stu-id="30b70-110">Type</span></span>|<span data-ttu-id="30b70-111">Описание</span><span class="sxs-lookup"><span data-stu-id="30b70-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30b70-112">key</span><span class="sxs-lookup"><span data-stu-id="30b70-112">key</span></span>|<span data-ttu-id="30b70-113">String.</span><span class="sxs-lookup"><span data-stu-id="30b70-113">String</span></span>|<span data-ttu-id="30b70-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="30b70-114">Key.</span></span>|
|<span data-ttu-id="30b70-115">value</span><span class="sxs-lookup"><span data-stu-id="30b70-115">value</span></span>|<span data-ttu-id="30b70-116">Строка</span><span class="sxs-lookup"><span data-stu-id="30b70-116">String</span></span>|<span data-ttu-id="30b70-117">Значение</span><span class="sxs-lookup"><span data-stu-id="30b70-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30b70-118">Связи</span><span class="sxs-lookup"><span data-stu-id="30b70-118">Relationships</span></span>
<span data-ttu-id="30b70-119">Нет</span><span class="sxs-lookup"><span data-stu-id="30b70-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30b70-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30b70-120">JSON Representation</span></span>
<span data-ttu-id="30b70-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30b70-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





