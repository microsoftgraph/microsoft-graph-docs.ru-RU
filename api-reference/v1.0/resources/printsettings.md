---
title: тип ресурса printSettings
description: Представляет параметры для службы универсальной печати для клиента.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 53e0db2a1923cad0af1f35baf5bed6fecd896fb3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517457"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="37b8d-103">тип ресурса printSettings</span><span class="sxs-lookup"><span data-stu-id="37b8d-103">printSettings resource type</span></span>

<span data-ttu-id="37b8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37b8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="37b8d-105">Представляет параметры для службы универсальной печати для клиента.</span><span class="sxs-lookup"><span data-stu-id="37b8d-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="37b8d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="37b8d-106">Properties</span></span>
|<span data-ttu-id="37b8d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="37b8d-107">Property</span></span>|<span data-ttu-id="37b8d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="37b8d-108">Type</span></span>|<span data-ttu-id="37b8d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="37b8d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37b8d-110">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="37b8d-110">documentConversionEnabled</span></span>|<span data-ttu-id="37b8d-111">Логический</span><span class="sxs-lookup"><span data-stu-id="37b8d-111">Boolean</span></span>|<span data-ttu-id="37b8d-112">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="37b8d-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="37b8d-113">Если преобразование документов включено, служба универсальной печати автоматически преобразует документы в формат, совместимый с принтером (xps to pdf) при необходимости.</span><span class="sxs-lookup"><span data-stu-id="37b8d-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37b8d-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37b8d-114">JSON representation</span></span>
<span data-ttu-id="37b8d-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37b8d-115">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printSettings",
  "documentConversionEnabled": "Boolean"
}
```

