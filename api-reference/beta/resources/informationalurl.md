---
title: Тип ресурса informationalUrl
description: Сведения о базовой профиля приложения.
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513650"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="565c3-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="565c3-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="565c3-104">Сведения о базовой профиля приложения.</span><span class="sxs-lookup"><span data-stu-id="565c3-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="565c3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="565c3-105">Properties</span></span>

| <span data-ttu-id="565c3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="565c3-106">Property</span></span> | <span data-ttu-id="565c3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="565c3-107">Type</span></span> | <span data-ttu-id="565c3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="565c3-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="565c3-109">маркетинг</span><span class="sxs-lookup"><span data-stu-id="565c3-109">marketing</span></span>|<span data-ttu-id="565c3-110">String</span><span class="sxs-lookup"><span data-stu-id="565c3-110">String</span></span>| <span data-ttu-id="565c3-111">Ссылка на приложение маркетинговых страницы.</span><span class="sxs-lookup"><span data-stu-id="565c3-111">Link to the application's marketing page.</span></span> <span data-ttu-id="565c3-112">Пример: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="565c3-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="565c3-113">конфиденциальность</span><span class="sxs-lookup"><span data-stu-id="565c3-113">privacy</span></span>|<span data-ttu-id="565c3-114">String</span><span class="sxs-lookup"><span data-stu-id="565c3-114">String</span></span>| <span data-ttu-id="565c3-115">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="565c3-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="565c3-116">Пример: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="565c3-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="565c3-117">Поддержка</span><span class="sxs-lookup"><span data-stu-id="565c3-117">support</span></span>|<span data-ttu-id="565c3-118">String</span><span class="sxs-lookup"><span data-stu-id="565c3-118">String</span></span>| <span data-ttu-id="565c3-119">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="565c3-119">Link to the application's support page.</span></span> <span data-ttu-id="565c3-120">Пример: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="565c3-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="565c3-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="565c3-121">termsOfService</span></span>|<span data-ttu-id="565c3-122">String</span><span class="sxs-lookup"><span data-stu-id="565c3-122">String</span></span>| <span data-ttu-id="565c3-123">Ссылка на условия приложения службы оператора.</span><span class="sxs-lookup"><span data-stu-id="565c3-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="565c3-124">Пример: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="565c3-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="565c3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="565c3-125">JSON representation</span></span>
<span data-ttu-id="565c3-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="565c3-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/informationalurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
