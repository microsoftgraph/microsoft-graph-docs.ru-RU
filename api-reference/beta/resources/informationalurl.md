---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548711"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="430da-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="430da-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="430da-104">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="430da-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="430da-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="430da-105">Properties</span></span>

| <span data-ttu-id="430da-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="430da-106">Property</span></span> | <span data-ttu-id="430da-107">Тип</span><span class="sxs-lookup"><span data-stu-id="430da-107">Type</span></span> | <span data-ttu-id="430da-108">Описание</span><span class="sxs-lookup"><span data-stu-id="430da-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="430da-109">проведения</span><span class="sxs-lookup"><span data-stu-id="430da-109">marketing</span></span>|<span data-ttu-id="430da-110">String</span><span class="sxs-lookup"><span data-stu-id="430da-110">String</span></span>| <span data-ttu-id="430da-111">Ссылка на маркетинговую страницу приложения.</span><span class="sxs-lookup"><span data-stu-id="430da-111">Link to the application's marketing page.</span></span> <span data-ttu-id="430da-112">Пример: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="430da-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="430da-113">уведомление</span><span class="sxs-lookup"><span data-stu-id="430da-113">privacy</span></span>|<span data-ttu-id="430da-114">String</span><span class="sxs-lookup"><span data-stu-id="430da-114">String</span></span>| <span data-ttu-id="430da-115">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="430da-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="430da-116">Пример: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="430da-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="430da-117">поддержки</span><span class="sxs-lookup"><span data-stu-id="430da-117">support</span></span>|<span data-ttu-id="430da-118">String</span><span class="sxs-lookup"><span data-stu-id="430da-118">String</span></span>| <span data-ttu-id="430da-119">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="430da-119">Link to the application's support page.</span></span> <span data-ttu-id="430da-120">Пример: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="430da-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="430da-121">Термсофсервице</span><span class="sxs-lookup"><span data-stu-id="430da-121">termsOfService</span></span>|<span data-ttu-id="430da-122">String</span><span class="sxs-lookup"><span data-stu-id="430da-122">String</span></span>| <span data-ttu-id="430da-123">Ссылка на условия заявления приложения.</span><span class="sxs-lookup"><span data-stu-id="430da-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="430da-124">Пример: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="430da-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="430da-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="430da-125">JSON representation</span></span>
<span data-ttu-id="430da-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="430da-126">Here is a JSON representation of the resource.</span></span>

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
