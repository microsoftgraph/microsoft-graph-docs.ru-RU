---
title: Тип ресурса accessPackageLocalizedContent
description: Сложный тип, используемый для представления текста на разных локальных уровнях вместе с текстом по умолчанию.*
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91ef87428b4171317943e9ecf1ec92e959c7a62b
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720328"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a><span data-ttu-id="8bb31-103">Тип ресурса accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="8bb31-103">accessPackageLocalizedContent resource type</span></span>

<span data-ttu-id="8bb31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bb31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb31-105">Сложный тип, используемый для представления текста в нескольких локализованных формах.</span><span class="sxs-lookup"><span data-stu-id="8bb31-105">A complex type used to represent a text in multiple localalized forms.</span></span> <span data-ttu-id="8bb31-106">Он включает текст по умолчанию, который используется в любом случае, когда запрашиваемая локализация недоступна.</span><span class="sxs-lookup"><span data-stu-id="8bb31-106">It includes a default text, which is used in any case where the requested localization is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="8bb31-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bb31-107">Properties</span></span>
|<span data-ttu-id="8bb31-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bb31-108">Property</span></span>|<span data-ttu-id="8bb31-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb31-109">Type</span></span>|<span data-ttu-id="8bb31-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bb31-111">defaultText</span><span class="sxs-lookup"><span data-stu-id="8bb31-111">defaultText</span></span>|<span data-ttu-id="8bb31-112">String</span><span class="sxs-lookup"><span data-stu-id="8bb31-112">String</span></span>|<span data-ttu-id="8bb31-113">Строка отката, которая используется, когда запрашиваемая локализация недоступна.</span><span class="sxs-lookup"><span data-stu-id="8bb31-113">The fallback string, which is used when a requested localization is not available.</span></span> <span data-ttu-id="8bb31-114">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bb31-114">Required.</span></span> |
|<span data-ttu-id="8bb31-115">localizedTexts</span><span class="sxs-lookup"><span data-stu-id="8bb31-115">localizedTexts</span></span>|<span data-ttu-id="8bb31-116">[Коллекция accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md)</span><span class="sxs-lookup"><span data-stu-id="8bb31-116">[accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md) collection</span></span>|<span data-ttu-id="8bb31-117">Контент, представленный в формате для определенного локали.</span><span class="sxs-lookup"><span data-stu-id="8bb31-117">Content represented in a format for a specific locale.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8bb31-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="8bb31-118">Relationships</span></span>
<span data-ttu-id="8bb31-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8bb31-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bb31-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8bb31-120">JSON representation</span></span>
<span data-ttu-id="8bb31-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bb31-121">The following is a JSON representation of the resource.</span></span>
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
