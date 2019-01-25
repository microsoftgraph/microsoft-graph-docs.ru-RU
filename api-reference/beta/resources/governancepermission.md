---
title: Тип ресурса governancePermission
description: 'Представляет, governanceSubject имеет разрешение на доступ к определенным governanceResource.  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529840"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="cabdb-103">Тип ресурса governancePermission</span><span class="sxs-lookup"><span data-stu-id="cabdb-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cabdb-104">Представляет, [governanceSubject](../resources/governancesubject.md) имеет разрешение на доступ к определенным [governanceResource](../resources/governanceresource.md).</span><span class="sxs-lookup"><span data-stu-id="cabdb-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="cabdb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cabdb-105">Properties</span></span>
| <span data-ttu-id="cabdb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cabdb-106">Property</span></span>     | <span data-ttu-id="cabdb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cabdb-107">Type</span></span>   |<span data-ttu-id="cabdb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cabdb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cabdb-109">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="cabdb-109">accessLevel</span></span>|<span data-ttu-id="cabdb-110">String</span><span class="sxs-lookup"><span data-stu-id="cabdb-110">String</span></span>|<span data-ttu-id="cabdb-111">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="cabdb-111">The access level.</span></span> <span data-ttu-id="cabdb-112">Допустимые значения: ``None``, ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="cabdb-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="cabdb-113">isActive</span><span class="sxs-lookup"><span data-stu-id="cabdb-113">isActive</span></span>|<span data-ttu-id="cabdb-114">Логическое</span><span class="sxs-lookup"><span data-stu-id="cabdb-114">Boolean</span></span>|<span data-ttu-id="cabdb-115">Указывает, если инициатора запроса имеет назначения активная роль на уровне доступа.</span><span class="sxs-lookup"><span data-stu-id="cabdb-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="cabdb-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="cabdb-116">isEligible</span></span>|<span data-ttu-id="cabdb-117">Логическое</span><span class="sxs-lookup"><span data-stu-id="cabdb-117">Boolean</span></span>|<span data-ttu-id="cabdb-118">Указывает, имеет ли инициатора запроса все назначения ролей право на уровне доступа.</span><span class="sxs-lookup"><span data-stu-id="cabdb-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cabdb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cabdb-119">JSON representation</span></span>

<span data-ttu-id="cabdb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cabdb-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
