---
title: Тип ресурса requiredResourceAccess
description: Задает набор области разрешений OAuth 2.0 и роли приложения в разделе указанного ресурса, доступ к приложению. Указанной области разрешений OAuth 2.0 может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** ) при вызове ресурса приложения. Свойство **requiredResourceAccess** объекта приложения — это коллекция **ReqiredResourceAccess**.
ms.openlocfilehash: 937557f2f078ade1b336cfd00cd128d428d59cbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080857"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="4d7e5-105">Тип ресурса requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="4d7e5-105">requiredResourceAccess resource type</span></span>

> <span data-ttu-id="4d7e5-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d7e5-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d7e5-108">Задает набор области разрешений OAuth 2.0 и роли приложения в разделе указанного ресурса, доступ к приложению.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-108">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="4d7e5-109">Указанной области разрешений OAuth 2.0 может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** ) при вызове ресурса приложения.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-109">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="4d7e5-110">Свойство **requiredResourceAccess** объекта [приложения](application.md) — это коллекция **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-110">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4d7e5-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d7e5-111">JSON representation</span></span>

<span data-ttu-id="4d7e5-112">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a><span data-ttu-id="4d7e5-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d7e5-113">Properties</span></span>
| <span data-ttu-id="4d7e5-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d7e5-114">Property</span></span>     | <span data-ttu-id="4d7e5-115">Тип</span><span class="sxs-lookup"><span data-stu-id="4d7e5-115">Type</span></span>   |<span data-ttu-id="4d7e5-116">Description</span><span class="sxs-lookup"><span data-stu-id="4d7e5-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d7e5-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="4d7e5-117">resourceAccess</span></span>|<span data-ttu-id="4d7e5-118">[ResourceAccess](resourceaccess.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4d7e5-118">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="4d7e5-119">Список области разрешений OAuth2.0 и роли приложения, необходимых приложению из указанного ресурса.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-119">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="4d7e5-120">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="4d7e5-120">resourceAppId</span></span>|<span data-ttu-id="4d7e5-121">String</span><span class="sxs-lookup"><span data-stu-id="4d7e5-121">String</span></span>|<span data-ttu-id="4d7e5-122">Уникальный идентификатор для ресурса, доступ к приложению.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-122">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="4d7e5-123">Это должен быть равен **appId** , объявлен ресурсов для конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-123">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
