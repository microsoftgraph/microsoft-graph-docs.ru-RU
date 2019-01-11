---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: fa26b8046b81db70300b8ff40abcbd2b84f3f0c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832797"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="1df99-107">Тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="1df99-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="1df99-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1df99-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1df99-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1df99-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1df99-110">Представляет приложение и запрошенные разрешения для явного согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="1df99-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="1df99-111">Требуется администраторам предоставляются разрешения для приложения.</span><span class="sxs-lookup"><span data-stu-id="1df99-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="1df99-112">preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются.</span><span class="sxs-lookup"><span data-stu-id="1df99-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="1df99-113">Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="1df99-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="1df99-114">Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="1df99-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="1df99-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="1df99-115">Properties</span></span>

| <span data-ttu-id="1df99-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="1df99-116">Property</span></span> | <span data-ttu-id="1df99-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1df99-117">Type</span></span> | <span data-ttu-id="1df99-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1df99-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1df99-119">appId</span><span class="sxs-lookup"><span data-stu-id="1df99-119">appId</span></span>|<span data-ttu-id="1df99-120">String</span><span class="sxs-lookup"><span data-stu-id="1df99-120">String</span></span>| <span data-ttu-id="1df99-121">Уникальный идентификатор для приложения.</span><span class="sxs-lookup"><span data-stu-id="1df99-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="1df99-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="1df99-122">permissionIds</span></span>|<span data-ttu-id="1df99-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1df99-123">String collection</span></span>| <span data-ttu-id="1df99-124">Уникальный идентификатор для [publishedPermissionScope](permissionscope.md) или [роли приложения](approle.md) приложения требуется.</span><span class="sxs-lookup"><span data-stu-id="1df99-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1df99-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1df99-125">JSON representation</span></span>
<span data-ttu-id="1df99-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1df99-126">Here is a JSON representation of the resource.</span></span>

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
