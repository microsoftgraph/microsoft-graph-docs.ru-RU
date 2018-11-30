---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
ms.openlocfilehash: 900e3f4d8e24743ed75b15f7a57188b46630c9fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076069"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="e6680-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="e6680-103">omaSetting resource type</span></span>

> <span data-ttu-id="e6680-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6680-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6680-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6680-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6680-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e6680-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6680-107">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="e6680-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="e6680-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6680-108">Properties</span></span>
|<span data-ttu-id="e6680-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6680-109">Property</span></span>|<span data-ttu-id="e6680-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e6680-110">Type</span></span>|<span data-ttu-id="e6680-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e6680-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6680-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e6680-112">displayName</span></span>|<span data-ttu-id="e6680-113">String</span><span class="sxs-lookup"><span data-stu-id="e6680-113">String</span></span>|<span data-ttu-id="e6680-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="e6680-114">Display Name.</span></span>|
|<span data-ttu-id="e6680-115">описание</span><span class="sxs-lookup"><span data-stu-id="e6680-115">description</span></span>|<span data-ttu-id="e6680-116">String</span><span class="sxs-lookup"><span data-stu-id="e6680-116">String</span></span>|<span data-ttu-id="e6680-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="e6680-117">Description.</span></span>|
|<span data-ttu-id="e6680-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="e6680-118">omaUri</span></span>|<span data-ttu-id="e6680-119">String</span><span class="sxs-lookup"><span data-stu-id="e6680-119">String</span></span>|<span data-ttu-id="e6680-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="e6680-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6680-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e6680-121">Relationships</span></span>
<span data-ttu-id="e6680-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e6680-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6680-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6680-123">JSON Representation</span></span>
<span data-ttu-id="e6680-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6680-124">Here is a JSON representation of the resource.</span></span>
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





