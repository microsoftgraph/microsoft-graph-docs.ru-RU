---
title: Тип ресурса accessPackageLocalizedText
description: Сложный тип, используемый для представления строки на определенном языке.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9573ae4118f02abdba5686fd94da96da71d374c2
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720382"
---
# <a name="accesspackagelocalizedtext-resource-type"></a><span data-ttu-id="7302f-103">Тип ресурса accessPackageLocalizedText</span><span class="sxs-lookup"><span data-stu-id="7302f-103">accessPackageLocalizedText resource type</span></span>

<span data-ttu-id="7302f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7302f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7302f-105">Сложный тип, используемый для представления строки на определенном языке.</span><span class="sxs-lookup"><span data-stu-id="7302f-105">A complex type used to represent a string in a specific language.</span></span>

## <a name="properties"></a><span data-ttu-id="7302f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7302f-106">Properties</span></span>
|<span data-ttu-id="7302f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7302f-107">Property</span></span>|<span data-ttu-id="7302f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7302f-108">Type</span></span>|<span data-ttu-id="7302f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7302f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7302f-110">languageCode</span><span class="sxs-lookup"><span data-stu-id="7302f-110">languageCode</span></span>|<span data-ttu-id="7302f-111">String</span><span class="sxs-lookup"><span data-stu-id="7302f-111">String</span></span>|<span data-ttu-id="7302f-112">Код ISO для намечаемого языка.</span><span class="sxs-lookup"><span data-stu-id="7302f-112">The ISO code for the intended language.</span></span> <span data-ttu-id="7302f-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7302f-113">Required.</span></span> |
|<span data-ttu-id="7302f-114">текст</span><span class="sxs-lookup"><span data-stu-id="7302f-114">text</span></span>|<span data-ttu-id="7302f-115">String</span><span class="sxs-lookup"><span data-stu-id="7302f-115">String</span></span>|<span data-ttu-id="7302f-116">Текст на определенном языке.</span><span class="sxs-lookup"><span data-stu-id="7302f-116">The text in the specific language.</span></span> <span data-ttu-id="7302f-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7302f-117">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7302f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="7302f-118">Relationships</span></span>
<span data-ttu-id="7302f-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7302f-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7302f-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7302f-120">JSON representation</span></span>
<span data-ttu-id="7302f-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7302f-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedText",
  "text": "String",
  "languageCode": "String"
}
```
