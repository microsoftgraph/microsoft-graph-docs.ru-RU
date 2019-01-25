---
title: Тип ресурса resourceAccess
description: Задает область разрешений для OAuth 2.0 или роль приложения, требующие приложения. Свойство **resourceAccess** типа requiredResourceAccess — это коллекция **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519026"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="78b8e-104">Тип ресурса resourceAccess</span><span class="sxs-lookup"><span data-stu-id="78b8e-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78b8e-105">Задает область разрешений для OAuth 2.0 или роль приложения, требующие приложения.</span><span class="sxs-lookup"><span data-stu-id="78b8e-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="78b8e-106">Свойство **resourceAccess** типа [requiredResourceAccess](requiredresourceaccess.md) — это коллекция **ResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="78b8e-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="78b8e-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78b8e-107">JSON representation</span></span>

<span data-ttu-id="78b8e-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="78b8e-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="78b8e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="78b8e-109">Properties</span></span>
| <span data-ttu-id="78b8e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="78b8e-110">Property</span></span>     | <span data-ttu-id="78b8e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="78b8e-111">Type</span></span>   |<span data-ttu-id="78b8e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="78b8e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78b8e-113">id</span><span class="sxs-lookup"><span data-stu-id="78b8e-113">id</span></span>|<span data-ttu-id="78b8e-114">Guid</span><span class="sxs-lookup"><span data-stu-id="78b8e-114">Guid</span></span>|<span data-ttu-id="78b8e-115">Уникальный идентификатор для одного из экземпляров [oAuth2Permission](oauth2permission.md) или [роли приложения](approle.md) , которые предоставляет доступ к приложению ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78b8e-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="78b8e-116">type</span><span class="sxs-lookup"><span data-stu-id="78b8e-116">type</span></span>|<span data-ttu-id="78b8e-117">String</span><span class="sxs-lookup"><span data-stu-id="78b8e-117">String</span></span>|<span data-ttu-id="78b8e-118">Указывает, будет ли свойство **id** ссылается на [oAuth2Permission](oauth2permission.md) или [роли приложения](approle.md).</span><span class="sxs-lookup"><span data-stu-id="78b8e-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="78b8e-119">Возможные значения: «область» или «роли».</span><span class="sxs-lookup"><span data-stu-id="78b8e-119">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
