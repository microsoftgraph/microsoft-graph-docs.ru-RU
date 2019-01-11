---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b9abc7db7b6d2ad16aa13886905c348e6c8f01b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826476"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="d2fd6-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="d2fd6-103">omaSetting resource type</span></span>

> <span data-ttu-id="d2fd6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2fd6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2fd6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2fd6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2fd6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2fd6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2fd6-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d2fd6-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="d2fd6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2fd6-108">Properties</span></span>
|<span data-ttu-id="d2fd6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2fd6-109">Property</span></span>|<span data-ttu-id="d2fd6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d2fd6-110">Type</span></span>|<span data-ttu-id="d2fd6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d2fd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2fd6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d2fd6-112">displayName</span></span>|<span data-ttu-id="d2fd6-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d2fd6-113">String</span></span>|<span data-ttu-id="d2fd6-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d2fd6-114">Display Name.</span></span>|
|<span data-ttu-id="d2fd6-115">описание</span><span class="sxs-lookup"><span data-stu-id="d2fd6-115">description</span></span>|<span data-ttu-id="d2fd6-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d2fd6-116">String</span></span>|<span data-ttu-id="d2fd6-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="d2fd6-117">Description.</span></span>|
|<span data-ttu-id="d2fd6-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="d2fd6-118">omaUri</span></span>|<span data-ttu-id="d2fd6-119">Строка</span><span class="sxs-lookup"><span data-stu-id="d2fd6-119">String</span></span>|<span data-ttu-id="d2fd6-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="d2fd6-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2fd6-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d2fd6-121">Relationships</span></span>
<span data-ttu-id="d2fd6-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d2fd6-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2fd6-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2fd6-123">JSON Representation</span></span>
<span data-ttu-id="d2fd6-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2fd6-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





