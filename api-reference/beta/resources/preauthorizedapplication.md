---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: 22945589341066f4609d47773cb04426774648fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524550"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="038ae-107">Тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="038ae-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="038ae-108">Представляет приложение и запрошенные разрешения для явного согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="038ae-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="038ae-109">Требуется администраторам предоставляются разрешения для приложения.</span><span class="sxs-lookup"><span data-stu-id="038ae-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="038ae-110">preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются.</span><span class="sxs-lookup"><span data-stu-id="038ae-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="038ae-111">Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="038ae-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="038ae-112">Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="038ae-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="038ae-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="038ae-113">Properties</span></span>

| <span data-ttu-id="038ae-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="038ae-114">Property</span></span> | <span data-ttu-id="038ae-115">Тип</span><span class="sxs-lookup"><span data-stu-id="038ae-115">Type</span></span> | <span data-ttu-id="038ae-116">Описание</span><span class="sxs-lookup"><span data-stu-id="038ae-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="038ae-117">appId</span><span class="sxs-lookup"><span data-stu-id="038ae-117">appId</span></span>|<span data-ttu-id="038ae-118">String</span><span class="sxs-lookup"><span data-stu-id="038ae-118">String</span></span>| <span data-ttu-id="038ae-119">Уникальный идентификатор для приложения.</span><span class="sxs-lookup"><span data-stu-id="038ae-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="038ae-120">permissionIds</span><span class="sxs-lookup"><span data-stu-id="038ae-120">permissionIds</span></span>|<span data-ttu-id="038ae-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="038ae-121">String collection</span></span>| <span data-ttu-id="038ae-122">Уникальный идентификатор для [publishedPermissionScope](permissionscope.md) или [роли приложения](approle.md) приложения требуется.</span><span class="sxs-lookup"><span data-stu-id="038ae-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="038ae-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="038ae-123">JSON representation</span></span>
<span data-ttu-id="038ae-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="038ae-124">Here is a JSON representation of the resource.</span></span>

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
