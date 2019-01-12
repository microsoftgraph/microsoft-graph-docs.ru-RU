---
title: Тип ресурса keyValue
description: Определение значения ключа.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5027388b455a41bc5895009a4ce79ca195ab8340
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957881"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="d9d96-103">Тип ресурса keyValue</span><span class="sxs-lookup"><span data-stu-id="d9d96-103">keyValue resource type</span></span>

> <span data-ttu-id="d9d96-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d9d96-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9d96-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9d96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9d96-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d9d96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9d96-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="d9d96-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="d9d96-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9d96-108">Properties</span></span>
|<span data-ttu-id="d9d96-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9d96-109">Property</span></span>|<span data-ttu-id="d9d96-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d9d96-110">Type</span></span>|<span data-ttu-id="d9d96-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9d96-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9d96-112">key</span><span class="sxs-lookup"><span data-stu-id="d9d96-112">key</span></span>|<span data-ttu-id="d9d96-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d9d96-113">String</span></span>|<span data-ttu-id="d9d96-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="d9d96-114">Key.</span></span>|
|<span data-ttu-id="d9d96-115">value</span><span class="sxs-lookup"><span data-stu-id="d9d96-115">value</span></span>|<span data-ttu-id="d9d96-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d9d96-116">String</span></span>|<span data-ttu-id="d9d96-117">Значение</span><span class="sxs-lookup"><span data-stu-id="d9d96-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9d96-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d9d96-118">Relationships</span></span>
<span data-ttu-id="d9d96-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d9d96-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9d96-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9d96-120">JSON Representation</span></span>
<span data-ttu-id="d9d96-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9d96-121">Here is a JSON representation of the resource.</span></span>
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





