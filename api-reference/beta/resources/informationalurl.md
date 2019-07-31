---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9e2eaad003f4669623a4db4af1b364e05198515d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006257"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="d4799-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="d4799-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4799-104">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="d4799-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="d4799-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4799-105">Properties</span></span>

| <span data-ttu-id="d4799-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4799-106">Property</span></span> | <span data-ttu-id="d4799-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d4799-107">Type</span></span> | <span data-ttu-id="d4799-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d4799-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d4799-109">проведения</span><span class="sxs-lookup"><span data-stu-id="d4799-109">marketing</span></span>|<span data-ttu-id="d4799-110">String</span><span class="sxs-lookup"><span data-stu-id="d4799-110">String</span></span>| <span data-ttu-id="d4799-111">Ссылка на маркетинговую страницу приложения.</span><span class="sxs-lookup"><span data-stu-id="d4799-111">Link to the application's marketing page.</span></span> <span data-ttu-id="d4799-112">Пример: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="d4799-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="d4799-113">уведомление</span><span class="sxs-lookup"><span data-stu-id="d4799-113">privacy</span></span>|<span data-ttu-id="d4799-114">String</span><span class="sxs-lookup"><span data-stu-id="d4799-114">String</span></span>| <span data-ttu-id="d4799-115">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="d4799-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="d4799-116">Пример: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="d4799-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="d4799-117">поддержки</span><span class="sxs-lookup"><span data-stu-id="d4799-117">support</span></span>|<span data-ttu-id="d4799-118">String</span><span class="sxs-lookup"><span data-stu-id="d4799-118">String</span></span>| <span data-ttu-id="d4799-119">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="d4799-119">Link to the application's support page.</span></span> <span data-ttu-id="d4799-120">Пример: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="d4799-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="d4799-121">Термсофсервице</span><span class="sxs-lookup"><span data-stu-id="d4799-121">termsOfService</span></span>|<span data-ttu-id="d4799-122">String</span><span class="sxs-lookup"><span data-stu-id="d4799-122">String</span></span>| <span data-ttu-id="d4799-123">Ссылка на условия заявления приложения.</span><span class="sxs-lookup"><span data-stu-id="d4799-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="d4799-124">Пример: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="d4799-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4799-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4799-125">JSON representation</span></span>
<span data-ttu-id="d4799-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4799-126">Here is a JSON representation of the resource.</span></span>

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
