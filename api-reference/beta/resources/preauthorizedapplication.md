---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрашиваемые разрешения для неявного согласия. Необходимо, чтобы администратор предоставил согласие на применение приложения. Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями. Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя. Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7adaf4fe960b762b12f6b2cc8607e64c9813712e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965819"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="eab19-107">Тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="eab19-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eab19-108">Представляет приложение и запрашиваемые разрешения для неявного согласия.</span><span class="sxs-lookup"><span data-stu-id="eab19-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="eab19-109">Необходимо, чтобы администратор предоставил согласие на применение приложения.</span><span class="sxs-lookup"><span data-stu-id="eab19-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="eab19-110">Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="eab19-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="eab19-111">Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="eab19-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="eab19-112">Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="eab19-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="eab19-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="eab19-113">Properties</span></span>

| <span data-ttu-id="eab19-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="eab19-114">Property</span></span> | <span data-ttu-id="eab19-115">Тип</span><span class="sxs-lookup"><span data-stu-id="eab19-115">Type</span></span> | <span data-ttu-id="eab19-116">Описание</span><span class="sxs-lookup"><span data-stu-id="eab19-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eab19-117">appId</span><span class="sxs-lookup"><span data-stu-id="eab19-117">appId</span></span>|<span data-ttu-id="eab19-118">String</span><span class="sxs-lookup"><span data-stu-id="eab19-118">String</span></span>| <span data-ttu-id="eab19-119">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="eab19-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="eab19-120">Пермиссионидс</span><span class="sxs-lookup"><span data-stu-id="eab19-120">permissionIds</span></span>|<span data-ttu-id="eab19-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="eab19-121">String collection</span></span>| <span data-ttu-id="eab19-122">Уникальный идентификатор для [публишедпермиссионскопе](permissionscope.md) или [аппроле](approle.md) , необходимых для приложения.</span><span class="sxs-lookup"><span data-stu-id="eab19-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eab19-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eab19-123">JSON representation</span></span>
<span data-ttu-id="eab19-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eab19-124">Here is a JSON representation of the resource.</span></span>

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
