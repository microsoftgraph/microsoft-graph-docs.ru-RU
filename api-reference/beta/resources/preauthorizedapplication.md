---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.
ms.openlocfilehash: d299aefcac541407e0e42d0b0933e903afa3e84d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082428"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="173d3-107">Тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="173d3-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="173d3-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="173d3-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="173d3-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="173d3-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="173d3-110">Представляет приложение и запрошенные разрешения для явного согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="173d3-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="173d3-111">Требуется администраторам предоставляются разрешения для приложения.</span><span class="sxs-lookup"><span data-stu-id="173d3-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="173d3-112">preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются.</span><span class="sxs-lookup"><span data-stu-id="173d3-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="173d3-113">Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="173d3-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="173d3-114">Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="173d3-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="173d3-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="173d3-115">Properties</span></span>

| <span data-ttu-id="173d3-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="173d3-116">Property</span></span> | <span data-ttu-id="173d3-117">Тип</span><span class="sxs-lookup"><span data-stu-id="173d3-117">Type</span></span> | <span data-ttu-id="173d3-118">Description</span><span class="sxs-lookup"><span data-stu-id="173d3-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="173d3-119">appId</span><span class="sxs-lookup"><span data-stu-id="173d3-119">appId</span></span>|<span data-ttu-id="173d3-120">String</span><span class="sxs-lookup"><span data-stu-id="173d3-120">String</span></span>| <span data-ttu-id="173d3-121">Уникальный идентификатор для приложения.</span><span class="sxs-lookup"><span data-stu-id="173d3-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="173d3-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="173d3-122">permissionIds</span></span>|<span data-ttu-id="173d3-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="173d3-123">String collection</span></span>| <span data-ttu-id="173d3-124">Уникальный идентификатор для [publishedPermissionScope](permissionscope.md) или [роли приложения](approle.md) приложения требуется.</span><span class="sxs-lookup"><span data-stu-id="173d3-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="173d3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="173d3-125">JSON representation</span></span>
<span data-ttu-id="173d3-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="173d3-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->