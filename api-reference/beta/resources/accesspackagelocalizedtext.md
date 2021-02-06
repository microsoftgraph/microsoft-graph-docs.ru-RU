---
title: Тип ресурса accessPackageLocalizedText
description: Сложный тип, используемый для представления строки на определенном языке.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8d493f0909617dcda26546ccc262d7591c6b9309
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137349"
---
# <a name="accesspackagelocalizedtext-resource-type"></a><span data-ttu-id="a94ba-103">Тип ресурса accessPackageLocalizedText</span><span class="sxs-lookup"><span data-stu-id="a94ba-103">accessPackageLocalizedText resource type</span></span>

<span data-ttu-id="a94ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a94ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a94ba-105">Сложный тип, используемый для представления строки на определенном языке.</span><span class="sxs-lookup"><span data-stu-id="a94ba-105">A complex type used to represent a string in a specific language.</span></span>

## <a name="properties"></a><span data-ttu-id="a94ba-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a94ba-106">Properties</span></span>
|<span data-ttu-id="a94ba-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a94ba-107">Property</span></span>|<span data-ttu-id="a94ba-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a94ba-108">Type</span></span>|<span data-ttu-id="a94ba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a94ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a94ba-110">languageCode</span><span class="sxs-lookup"><span data-stu-id="a94ba-110">languageCode</span></span>|<span data-ttu-id="a94ba-111">Строка</span><span class="sxs-lookup"><span data-stu-id="a94ba-111">String</span></span>|<span data-ttu-id="a94ba-112">Код ISO для намечаемого языка.</span><span class="sxs-lookup"><span data-stu-id="a94ba-112">The ISO code for the intended language.</span></span> <span data-ttu-id="a94ba-113">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="a94ba-113">Required.</span></span> |
|<span data-ttu-id="a94ba-114">текст</span><span class="sxs-lookup"><span data-stu-id="a94ba-114">text</span></span>|<span data-ttu-id="a94ba-115">Строка</span><span class="sxs-lookup"><span data-stu-id="a94ba-115">String</span></span>|<span data-ttu-id="a94ba-116">Текст на определенном языке.</span><span class="sxs-lookup"><span data-stu-id="a94ba-116">The text in the specific language.</span></span> <span data-ttu-id="a94ba-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a94ba-117">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a94ba-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a94ba-118">Relationships</span></span>
<span data-ttu-id="a94ba-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a94ba-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a94ba-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a94ba-120">JSON representation</span></span>
<span data-ttu-id="a94ba-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a94ba-121">The following is a JSON representation of the resource.</span></span>
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
