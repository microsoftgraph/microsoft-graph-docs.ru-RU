---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрашиваемые разрешения для неявного согласия. Необходимо, чтобы администратор предоставил согласие на применение приложения. Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями. Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя. Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: f74ac0883c883bfbb2cb93c2da58e9fd8419dadd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344236"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="b1deb-107">Тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="b1deb-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1deb-108">Представляет приложение и запрашиваемые разрешения для неявного согласия.</span><span class="sxs-lookup"><span data-stu-id="b1deb-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="b1deb-109">Необходимо, чтобы администратор предоставил согласие на применение приложения.</span><span class="sxs-lookup"><span data-stu-id="b1deb-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="b1deb-110">Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="b1deb-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="b1deb-111">Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1deb-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="b1deb-112">Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1deb-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="b1deb-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1deb-113">Properties</span></span>

| <span data-ttu-id="b1deb-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1deb-114">Property</span></span> | <span data-ttu-id="b1deb-115">Тип</span><span class="sxs-lookup"><span data-stu-id="b1deb-115">Type</span></span> | <span data-ttu-id="b1deb-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b1deb-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b1deb-117">appId</span><span class="sxs-lookup"><span data-stu-id="b1deb-117">appId</span></span>|<span data-ttu-id="b1deb-118">String</span><span class="sxs-lookup"><span data-stu-id="b1deb-118">String</span></span>| <span data-ttu-id="b1deb-119">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="b1deb-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="b1deb-120">Пермиссионидс</span><span class="sxs-lookup"><span data-stu-id="b1deb-120">permissionIds</span></span>|<span data-ttu-id="b1deb-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b1deb-121">String collection</span></span>| <span data-ttu-id="b1deb-122">Уникальный идентификатор для [публишедпермиссионскопе](permissionscope.md) или [аппроле](approle.md) , необходимых для приложения.</span><span class="sxs-lookup"><span data-stu-id="b1deb-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1deb-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1deb-123">JSON representation</span></span>
<span data-ttu-id="b1deb-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1deb-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
