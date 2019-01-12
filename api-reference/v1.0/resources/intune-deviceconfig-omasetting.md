---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42b6d5fcea7b3b46acf8d0a119213f679d99aed6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961486"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="3a6dc-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="3a6dc-103">omaSetting resource type</span></span>

> <span data-ttu-id="3a6dc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3a6dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a6dc-105">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="3a6dc-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="3a6dc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a6dc-106">Properties</span></span>
|<span data-ttu-id="3a6dc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a6dc-107">Property</span></span>|<span data-ttu-id="3a6dc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3a6dc-108">Type</span></span>|<span data-ttu-id="3a6dc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3a6dc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a6dc-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3a6dc-110">displayName</span></span>|<span data-ttu-id="3a6dc-111">Строка</span><span class="sxs-lookup"><span data-stu-id="3a6dc-111">String</span></span>|<span data-ttu-id="3a6dc-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3a6dc-112">Display Name.</span></span>|
|<span data-ttu-id="3a6dc-113">описание</span><span class="sxs-lookup"><span data-stu-id="3a6dc-113">description</span></span>|<span data-ttu-id="3a6dc-114">Строка</span><span class="sxs-lookup"><span data-stu-id="3a6dc-114">String</span></span>|<span data-ttu-id="3a6dc-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="3a6dc-115">Description.</span></span>|
|<span data-ttu-id="3a6dc-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="3a6dc-116">omaUri</span></span>|<span data-ttu-id="3a6dc-117">Строка</span><span class="sxs-lookup"><span data-stu-id="3a6dc-117">String</span></span>|<span data-ttu-id="3a6dc-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="3a6dc-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a6dc-119">Связи</span><span class="sxs-lookup"><span data-stu-id="3a6dc-119">Relationships</span></span>
<span data-ttu-id="3a6dc-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3a6dc-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a6dc-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a6dc-121">JSON Representation</span></span>
<span data-ttu-id="3a6dc-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a6dc-122">Here is a JSON representation of the resource.</span></span>
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



