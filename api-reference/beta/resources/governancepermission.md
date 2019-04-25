---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547510"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="7bedc-103">Тип ресурса Говернанцепермиссион</span><span class="sxs-lookup"><span data-stu-id="7bedc-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bedc-104">Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .</span><span class="sxs-lookup"><span data-stu-id="7bedc-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="7bedc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bedc-105">Properties</span></span>
| <span data-ttu-id="7bedc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bedc-106">Property</span></span>     | <span data-ttu-id="7bedc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7bedc-107">Type</span></span>   |<span data-ttu-id="7bedc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7bedc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bedc-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="7bedc-109">accessLevel</span></span>|<span data-ttu-id="7bedc-110">String</span><span class="sxs-lookup"><span data-stu-id="7bedc-110">String</span></span>|<span data-ttu-id="7bedc-111">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="7bedc-111">The access level.</span></span> <span data-ttu-id="7bedc-112">Допустимые значения ``None``: ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="7bedc-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="7bedc-113">isActive</span><span class="sxs-lookup"><span data-stu-id="7bedc-113">isActive</span></span>|<span data-ttu-id="7bedc-114">Логический</span><span class="sxs-lookup"><span data-stu-id="7bedc-114">Boolean</span></span>|<span data-ttu-id="7bedc-115">Указывает, имеет ли запрашивающая сторона какое – либо активное назначение ролей для этого уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="7bedc-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="7bedc-116">Действительный</span><span class="sxs-lookup"><span data-stu-id="7bedc-116">isEligible</span></span>|<span data-ttu-id="7bedc-117">Логический</span><span class="sxs-lookup"><span data-stu-id="7bedc-117">Boolean</span></span>|<span data-ttu-id="7bedc-118">Указывает, имеет ли запрашивающее назначение роли для уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="7bedc-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bedc-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7bedc-119">JSON representation</span></span>

<span data-ttu-id="7bedc-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bedc-120">Here is a JSON representation of the resource.</span></span>

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
