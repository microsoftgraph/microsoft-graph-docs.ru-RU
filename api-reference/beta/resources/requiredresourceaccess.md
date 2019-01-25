---
title: Тип ресурса requiredResourceAccess
description: Задает набор области разрешений OAuth 2.0 и роли приложения в разделе указанного ресурса, доступ к приложению. Указанной области разрешений OAuth 2.0 может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** ) при вызове ресурса приложения. Свойство **requiredResourceAccess** объекта приложения — это коллекция **ReqiredResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512971"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="1f3f7-105">Тип ресурса requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="1f3f7-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f3f7-106">Задает набор области разрешений OAuth 2.0 и роли приложения в разделе указанного ресурса, доступ к приложению.</span><span class="sxs-lookup"><span data-stu-id="1f3f7-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="1f3f7-107">Указанной области разрешений OAuth 2.0 может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** ) при вызове ресурса приложения.</span><span class="sxs-lookup"><span data-stu-id="1f3f7-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="1f3f7-108">Свойство **requiredResourceAccess** объекта [приложения](application.md) — это коллекция **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="1f3f7-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1f3f7-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f3f7-109">JSON representation</span></span>

<span data-ttu-id="1f3f7-110">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="1f3f7-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="1f3f7-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f3f7-111">Properties</span></span>
| <span data-ttu-id="1f3f7-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f3f7-112">Property</span></span>     | <span data-ttu-id="1f3f7-113">Тип</span><span class="sxs-lookup"><span data-stu-id="1f3f7-113">Type</span></span>   |<span data-ttu-id="1f3f7-114">Описание</span><span class="sxs-lookup"><span data-stu-id="1f3f7-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f3f7-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="1f3f7-115">resourceAccess</span></span>|<span data-ttu-id="1f3f7-116">[ResourceAccess](resourceaccess.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1f3f7-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="1f3f7-117">Список области разрешений OAuth2.0 и роли приложения, необходимых приложению из указанного ресурса.</span><span class="sxs-lookup"><span data-stu-id="1f3f7-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="1f3f7-118">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="1f3f7-118">resourceAppId</span></span>|<span data-ttu-id="1f3f7-119">String</span><span class="sxs-lookup"><span data-stu-id="1f3f7-119">String</span></span>|<span data-ttu-id="1f3f7-120">Уникальный идентификатор для ресурса, доступ к приложению.</span><span class="sxs-lookup"><span data-stu-id="1f3f7-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="1f3f7-121">Это должен быть равен **appId** , объявлен ресурсов для конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="1f3f7-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
