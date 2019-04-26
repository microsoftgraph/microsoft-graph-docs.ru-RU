---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
ms.openlocfilehash: c858bb55db083510661edfc36f32b9a511c5e6f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340012"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="51ed7-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="51ed7-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51ed7-104">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="51ed7-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="51ed7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="51ed7-105">Properties</span></span>

| <span data-ttu-id="51ed7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="51ed7-106">Property</span></span> | <span data-ttu-id="51ed7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="51ed7-107">Type</span></span> | <span data-ttu-id="51ed7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51ed7-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="51ed7-109">проведения</span><span class="sxs-lookup"><span data-stu-id="51ed7-109">marketing</span></span>|<span data-ttu-id="51ed7-110">String</span><span class="sxs-lookup"><span data-stu-id="51ed7-110">String</span></span>| <span data-ttu-id="51ed7-111">Ссылка на маркетинговую страницу приложения.</span><span class="sxs-lookup"><span data-stu-id="51ed7-111">Link to the application's marketing page.</span></span> <span data-ttu-id="51ed7-112">Пример: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="51ed7-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="51ed7-113">уведомление</span><span class="sxs-lookup"><span data-stu-id="51ed7-113">privacy</span></span>|<span data-ttu-id="51ed7-114">String</span><span class="sxs-lookup"><span data-stu-id="51ed7-114">String</span></span>| <span data-ttu-id="51ed7-115">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="51ed7-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="51ed7-116">Пример: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="51ed7-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="51ed7-117">поддержки</span><span class="sxs-lookup"><span data-stu-id="51ed7-117">support</span></span>|<span data-ttu-id="51ed7-118">String</span><span class="sxs-lookup"><span data-stu-id="51ed7-118">String</span></span>| <span data-ttu-id="51ed7-119">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="51ed7-119">Link to the application's support page.</span></span> <span data-ttu-id="51ed7-120">Пример: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="51ed7-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="51ed7-121">Термсофсервице</span><span class="sxs-lookup"><span data-stu-id="51ed7-121">termsOfService</span></span>|<span data-ttu-id="51ed7-122">String</span><span class="sxs-lookup"><span data-stu-id="51ed7-122">String</span></span>| <span data-ttu-id="51ed7-123">Ссылка на условия заявления приложения.</span><span class="sxs-lookup"><span data-stu-id="51ed7-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="51ed7-124">Пример: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="51ed7-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51ed7-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51ed7-125">JSON representation</span></span>
<span data-ttu-id="51ed7-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51ed7-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
