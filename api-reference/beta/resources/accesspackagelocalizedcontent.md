---
title: Тип ресурса accessPackageLocalizedContent
description: Сложный тип, используемый для представления текста на разных локальных уровнях вместе с текстом по умолчанию.*
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 155d0ffd8f7f705c79bd753aa26f659968b87829
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137356"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a><span data-ttu-id="e331b-103">Тип ресурса accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="e331b-103">accessPackageLocalizedContent resource type</span></span>

<span data-ttu-id="e331b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e331b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e331b-105">Сложный тип, используемый для представления текста в нескольких локализованных формах.</span><span class="sxs-lookup"><span data-stu-id="e331b-105">A complex type used to represent a text in multiple localalized forms.</span></span> <span data-ttu-id="e331b-106">Он включает текст по умолчанию, который используется в любом случае, когда запрашиваемая локализация недоступна.</span><span class="sxs-lookup"><span data-stu-id="e331b-106">It includes a default text, which is used in any case where the requested localization is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="e331b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e331b-107">Properties</span></span>
|<span data-ttu-id="e331b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e331b-108">Property</span></span>|<span data-ttu-id="e331b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e331b-109">Type</span></span>|<span data-ttu-id="e331b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e331b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e331b-111">defaultText</span><span class="sxs-lookup"><span data-stu-id="e331b-111">defaultText</span></span>|<span data-ttu-id="e331b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e331b-112">String</span></span>|<span data-ttu-id="e331b-113">Строка отката, которая используется, когда запрашиваемая локализация недоступна.</span><span class="sxs-lookup"><span data-stu-id="e331b-113">The fallback string, which is used when a requested localization is not available.</span></span> <span data-ttu-id="e331b-114">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e331b-114">Required.</span></span> |
|<span data-ttu-id="e331b-115">localizedTexts</span><span class="sxs-lookup"><span data-stu-id="e331b-115">localizedTexts</span></span>|<span data-ttu-id="e331b-116">[Коллекция accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md)</span><span class="sxs-lookup"><span data-stu-id="e331b-116">[accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md) collection</span></span>|<span data-ttu-id="e331b-117">Контент, представленный в формате для определенного локали.</span><span class="sxs-lookup"><span data-stu-id="e331b-117">Content represented in a format for a specific locale.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e331b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e331b-118">Relationships</span></span>
<span data-ttu-id="e331b-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e331b-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e331b-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e331b-120">JSON representation</span></span>
<span data-ttu-id="e331b-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e331b-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedContent",
  "defaultText": "String",
  "localizedTexts": [
    {
      "@odata.type": "microsoft.graph.accessPackageLocalizedText"
    }
  ]
}
```
