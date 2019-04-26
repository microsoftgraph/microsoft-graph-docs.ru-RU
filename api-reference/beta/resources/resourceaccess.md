---
title: Тип ресурса Ресаурцеакцесс
description: Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением. Свойство **ресаурцеакцесс** типа рекуиредресаурцеакцесс является коллекцией **ресаурцеакцесс**.
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563065"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="3011f-104">Тип ресурса Ресаурцеакцесс</span><span class="sxs-lookup"><span data-stu-id="3011f-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3011f-105">Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением.</span><span class="sxs-lookup"><span data-stu-id="3011f-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="3011f-106">Свойство **ресаурцеакцесс** типа [рекуиредресаурцеакцесс](requiredresourceaccess.md) является коллекцией **ресаурцеакцесс**.</span><span class="sxs-lookup"><span data-stu-id="3011f-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3011f-107">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3011f-107">JSON representation</span></span>

<span data-ttu-id="3011f-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3011f-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3011f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3011f-109">Properties</span></span>
| <span data-ttu-id="3011f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3011f-110">Property</span></span>     | <span data-ttu-id="3011f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3011f-111">Type</span></span>   |<span data-ttu-id="3011f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3011f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3011f-113">id</span><span class="sxs-lookup"><span data-stu-id="3011f-113">id</span></span>|<span data-ttu-id="3011f-114">Guid</span><span class="sxs-lookup"><span data-stu-id="3011f-114">Guid</span></span>|<span data-ttu-id="3011f-115">Уникальный идентификатор для одного из экземпляров [oAuth2Permission](oauth2permission.md) или [аппроле](approle.md) , предоставляемых приложением ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3011f-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="3011f-116">type</span><span class="sxs-lookup"><span data-stu-id="3011f-116">type</span></span>|<span data-ttu-id="3011f-117">String</span><span class="sxs-lookup"><span data-stu-id="3011f-117">String</span></span>|<span data-ttu-id="3011f-118">Указывает, ссылается ли свойство **ID** на объект [oAuth2Permission](oauth2permission.md) или [аппроле](approle.md).</span><span class="sxs-lookup"><span data-stu-id="3011f-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="3011f-119">Возможные значения: "Scope" или "role".</span><span class="sxs-lookup"><span data-stu-id="3011f-119">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
