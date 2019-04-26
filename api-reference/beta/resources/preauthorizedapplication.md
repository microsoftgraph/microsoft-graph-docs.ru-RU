---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрашиваемые разрешения для неявного согласия. Необходимо, чтобы администратор предоставил согласие на применение приложения. Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями. Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя. Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: 22945589341066f4609d47773cb04426774648fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563632"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="03ce0-107">Тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="03ce0-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03ce0-108">Представляет приложение и запрашиваемые разрешения для неявного согласия.</span><span class="sxs-lookup"><span data-stu-id="03ce0-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="03ce0-109">Необходимо, чтобы администратор предоставил согласие на применение приложения.</span><span class="sxs-lookup"><span data-stu-id="03ce0-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="03ce0-110">Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="03ce0-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="03ce0-111">Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="03ce0-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="03ce0-112">Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="03ce0-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="03ce0-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="03ce0-113">Properties</span></span>

| <span data-ttu-id="03ce0-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="03ce0-114">Property</span></span> | <span data-ttu-id="03ce0-115">Тип</span><span class="sxs-lookup"><span data-stu-id="03ce0-115">Type</span></span> | <span data-ttu-id="03ce0-116">Описание</span><span class="sxs-lookup"><span data-stu-id="03ce0-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="03ce0-117">appId</span><span class="sxs-lookup"><span data-stu-id="03ce0-117">appId</span></span>|<span data-ttu-id="03ce0-118">String</span><span class="sxs-lookup"><span data-stu-id="03ce0-118">String</span></span>| <span data-ttu-id="03ce0-119">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="03ce0-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="03ce0-120">Пермиссионидс</span><span class="sxs-lookup"><span data-stu-id="03ce0-120">permissionIds</span></span>|<span data-ttu-id="03ce0-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="03ce0-121">String collection</span></span>| <span data-ttu-id="03ce0-122">Уникальный идентификатор для [публишедпермиссионскопе](permissionscope.md) или [аппроле](approle.md) , необходимых для приложения.</span><span class="sxs-lookup"><span data-stu-id="03ce0-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03ce0-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03ce0-123">JSON representation</span></span>
<span data-ttu-id="03ce0-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03ce0-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/preauthorizedapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
