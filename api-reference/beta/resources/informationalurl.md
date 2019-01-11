---
title: Тип ресурса informationalUrl
description: Сведения о базовой профиля приложения.
localization_priority: Normal
ms.openlocfilehash: 78fd03a2673b342d1a0c904f521fe5a0f8cba205
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816984"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="a5a3b-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="a5a3b-103">informationalUrl resource type</span></span>

> <span data-ttu-id="a5a3b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5a3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5a3b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a3b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5a3b-106">Сведения о базовой профиля приложения.</span><span class="sxs-lookup"><span data-stu-id="a5a3b-106">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="a5a3b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5a3b-107">Properties</span></span>

| <span data-ttu-id="a5a3b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5a3b-108">Property</span></span> | <span data-ttu-id="a5a3b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a5a3b-109">Type</span></span> | <span data-ttu-id="a5a3b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5a3b-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a5a3b-111">маркетинг</span><span class="sxs-lookup"><span data-stu-id="a5a3b-111">marketing</span></span>|<span data-ttu-id="a5a3b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a5a3b-112">String</span></span>| <span data-ttu-id="a5a3b-113">Ссылка на приложение маркетинговых страницы.</span><span class="sxs-lookup"><span data-stu-id="a5a3b-113">Link to the application's marketing page.</span></span> <span data-ttu-id="a5a3b-114">Например, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="a5a3b-114">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="a5a3b-115">конфиденциальность</span><span class="sxs-lookup"><span data-stu-id="a5a3b-115">privacy</span></span>|<span data-ttu-id="a5a3b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a5a3b-116">String</span></span>| <span data-ttu-id="a5a3b-117">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="a5a3b-117">Link to the application's privacy statement.</span></span> <span data-ttu-id="a5a3b-118">Например, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="a5a3b-118">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="a5a3b-119">Поддержка</span><span class="sxs-lookup"><span data-stu-id="a5a3b-119">support</span></span>|<span data-ttu-id="a5a3b-120">Строка</span><span class="sxs-lookup"><span data-stu-id="a5a3b-120">String</span></span>| <span data-ttu-id="a5a3b-121">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="a5a3b-121">Link to the application's support page.</span></span> <span data-ttu-id="a5a3b-122">Например, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="a5a3b-122">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="a5a3b-123">termsOfService</span><span class="sxs-lookup"><span data-stu-id="a5a3b-123">termsOfService</span></span>|<span data-ttu-id="a5a3b-124">Строка</span><span class="sxs-lookup"><span data-stu-id="a5a3b-124">String</span></span>| <span data-ttu-id="a5a3b-125">Ссылка на условия приложения службы оператора.</span><span class="sxs-lookup"><span data-stu-id="a5a3b-125">Link to the application's terms of service statement.</span></span> <span data-ttu-id="a5a3b-126">Например, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="a5a3b-126">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5a3b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5a3b-127">JSON representation</span></span>
<span data-ttu-id="a5a3b-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5a3b-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
