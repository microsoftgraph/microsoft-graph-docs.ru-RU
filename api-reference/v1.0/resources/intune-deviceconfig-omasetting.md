---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
ms.openlocfilehash: 7ef8617ca4ce10ebeabf0d7a4655688e58925646
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025790"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="36b3d-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="36b3d-103">omaSetting resource type</span></span>

> <span data-ttu-id="36b3d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36b3d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36b3d-105">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="36b3d-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="36b3d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="36b3d-106">Properties</span></span>
|<span data-ttu-id="36b3d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="36b3d-107">Property</span></span>|<span data-ttu-id="36b3d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="36b3d-108">Type</span></span>|<span data-ttu-id="36b3d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36b3d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36b3d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="36b3d-110">displayName</span></span>|<span data-ttu-id="36b3d-111">String</span><span class="sxs-lookup"><span data-stu-id="36b3d-111">String</span></span>|<span data-ttu-id="36b3d-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="36b3d-112">Display Name.</span></span>|
|<span data-ttu-id="36b3d-113">описание</span><span class="sxs-lookup"><span data-stu-id="36b3d-113">description</span></span>|<span data-ttu-id="36b3d-114">String</span><span class="sxs-lookup"><span data-stu-id="36b3d-114">String</span></span>|<span data-ttu-id="36b3d-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="36b3d-115">Description.</span></span>|
|<span data-ttu-id="36b3d-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="36b3d-116">omaUri</span></span>|<span data-ttu-id="36b3d-117">String</span><span class="sxs-lookup"><span data-stu-id="36b3d-117">String</span></span>|<span data-ttu-id="36b3d-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="36b3d-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36b3d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="36b3d-119">Relationships</span></span>
<span data-ttu-id="36b3d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="36b3d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="36b3d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36b3d-121">JSON Representation</span></span>
<span data-ttu-id="36b3d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36b3d-122">Here is a JSON representation of the resource.</span></span>
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



