---
title: Тип ресурса informationalUrl
description: Сведения о базовой профиля приложения.
ms.openlocfilehash: c8a13f4f686fe3b6ffd460ab05342b7da9b4a808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079866"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="08317-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="08317-103">informationalUrl resource type</span></span>

> <span data-ttu-id="08317-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08317-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08317-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08317-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08317-106">Сведения о базовой профиля приложения.</span><span class="sxs-lookup"><span data-stu-id="08317-106">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="08317-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08317-107">Properties</span></span>

| <span data-ttu-id="08317-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08317-108">Property</span></span> | <span data-ttu-id="08317-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08317-109">Type</span></span> | <span data-ttu-id="08317-110">Description</span><span class="sxs-lookup"><span data-stu-id="08317-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="08317-111">маркетинг</span><span class="sxs-lookup"><span data-stu-id="08317-111">marketing</span></span>|<span data-ttu-id="08317-112">String</span><span class="sxs-lookup"><span data-stu-id="08317-112">String</span></span>| <span data-ttu-id="08317-113">Ссылка на приложение маркетинговых страницы.</span><span class="sxs-lookup"><span data-stu-id="08317-113">Link to the application's marketing page.</span></span> <span data-ttu-id="08317-114">Например, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="08317-114">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="08317-115">конфиденциальность</span><span class="sxs-lookup"><span data-stu-id="08317-115">privacy</span></span>|<span data-ttu-id="08317-116">String</span><span class="sxs-lookup"><span data-stu-id="08317-116">String</span></span>| <span data-ttu-id="08317-117">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="08317-117">Link to the application's privacy statement.</span></span> <span data-ttu-id="08317-118">Например, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="08317-118">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="08317-119">Поддержка</span><span class="sxs-lookup"><span data-stu-id="08317-119">support</span></span>|<span data-ttu-id="08317-120">String</span><span class="sxs-lookup"><span data-stu-id="08317-120">String</span></span>| <span data-ttu-id="08317-121">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="08317-121">Link to the application's support page.</span></span> <span data-ttu-id="08317-122">Например, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="08317-122">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="08317-123">termsOfService</span><span class="sxs-lookup"><span data-stu-id="08317-123">termsOfService</span></span>|<span data-ttu-id="08317-124">String</span><span class="sxs-lookup"><span data-stu-id="08317-124">String</span></span>| <span data-ttu-id="08317-125">Ссылка на условия приложения службы оператора.</span><span class="sxs-lookup"><span data-stu-id="08317-125">Link to the application's terms of service statement.</span></span> <span data-ttu-id="08317-126">Например, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="08317-126">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08317-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08317-127">JSON representation</span></span>
<span data-ttu-id="08317-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08317-128">Here is a JSON representation of the resource.</span></span>

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