---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e6cb37078eb6c5b4aee00a9ac7bfc77061ec0bcf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946597"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="4e7eb-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="4e7eb-103">omaSetting resource type</span></span>

> <span data-ttu-id="4e7eb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e7eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e7eb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e7eb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4e7eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e7eb-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="4e7eb-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="4e7eb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e7eb-108">Properties</span></span>
|<span data-ttu-id="4e7eb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e7eb-109">Property</span></span>|<span data-ttu-id="4e7eb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4e7eb-110">Type</span></span>|<span data-ttu-id="4e7eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4e7eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e7eb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4e7eb-112">displayName</span></span>|<span data-ttu-id="4e7eb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="4e7eb-113">String</span></span>|<span data-ttu-id="4e7eb-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4e7eb-114">Display Name.</span></span>|
|<span data-ttu-id="4e7eb-115">описание</span><span class="sxs-lookup"><span data-stu-id="4e7eb-115">description</span></span>|<span data-ttu-id="4e7eb-116">Строка</span><span class="sxs-lookup"><span data-stu-id="4e7eb-116">String</span></span>|<span data-ttu-id="4e7eb-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="4e7eb-117">Description.</span></span>|
|<span data-ttu-id="4e7eb-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="4e7eb-118">omaUri</span></span>|<span data-ttu-id="4e7eb-119">Строка</span><span class="sxs-lookup"><span data-stu-id="4e7eb-119">String</span></span>|<span data-ttu-id="4e7eb-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="4e7eb-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e7eb-121">Связи</span><span class="sxs-lookup"><span data-stu-id="4e7eb-121">Relationships</span></span>
<span data-ttu-id="4e7eb-122">Нет</span><span class="sxs-lookup"><span data-stu-id="4e7eb-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4e7eb-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e7eb-123">JSON Representation</span></span>
<span data-ttu-id="4e7eb-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e7eb-124">Here is a JSON representation of the resource.</span></span>
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





