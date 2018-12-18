---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
ms.openlocfilehash: fa1fc438ef97357ebd5f13443077384bc98e24f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314044"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="78c6e-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="78c6e-103">omaSetting resource type</span></span>

> <span data-ttu-id="78c6e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78c6e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78c6e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78c6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78c6e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78c6e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78c6e-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="78c6e-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="78c6e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78c6e-108">Properties</span></span>
|<span data-ttu-id="78c6e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="78c6e-109">Property</span></span>|<span data-ttu-id="78c6e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78c6e-110">Type</span></span>|<span data-ttu-id="78c6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78c6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78c6e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="78c6e-112">displayName</span></span>|<span data-ttu-id="78c6e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="78c6e-113">String</span></span>|<span data-ttu-id="78c6e-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="78c6e-114">Display Name.</span></span>|
|<span data-ttu-id="78c6e-115">описание</span><span class="sxs-lookup"><span data-stu-id="78c6e-115">description</span></span>|<span data-ttu-id="78c6e-116">Строка</span><span class="sxs-lookup"><span data-stu-id="78c6e-116">String</span></span>|<span data-ttu-id="78c6e-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="78c6e-117">Description.</span></span>|
|<span data-ttu-id="78c6e-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="78c6e-118">omaUri</span></span>|<span data-ttu-id="78c6e-119">Строка</span><span class="sxs-lookup"><span data-stu-id="78c6e-119">String</span></span>|<span data-ttu-id="78c6e-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="78c6e-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78c6e-121">Связи</span><span class="sxs-lookup"><span data-stu-id="78c6e-121">Relationships</span></span>
<span data-ttu-id="78c6e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="78c6e-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78c6e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78c6e-123">JSON Representation</span></span>
<span data-ttu-id="78c6e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78c6e-124">Here is a JSON representation of the resource.</span></span>
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





