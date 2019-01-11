---
title: Тип ресурса resourceAccess
description: Задает область разрешений для OAuth 2.0 или роль приложения, требующие приложения. Свойство **resourceAccess** типа requiredResourceAccess — это коллекция **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: f5389915897c3aab8b8277a45b54042bc861b290
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862337"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="844c2-104">Тип ресурса resourceAccess</span><span class="sxs-lookup"><span data-stu-id="844c2-104">resourceAccess resource type</span></span>

> <span data-ttu-id="844c2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="844c2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="844c2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="844c2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="844c2-107">Задает область разрешений для OAuth 2.0 или роль приложения, требующие приложения.</span><span class="sxs-lookup"><span data-stu-id="844c2-107">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="844c2-108">Свойство **resourceAccess** типа [requiredResourceAccess](requiredresourceaccess.md) — это коллекция **ResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="844c2-108">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="844c2-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="844c2-109">JSON representation</span></span>

<span data-ttu-id="844c2-110">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="844c2-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="844c2-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="844c2-111">Properties</span></span>
| <span data-ttu-id="844c2-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="844c2-112">Property</span></span>     | <span data-ttu-id="844c2-113">Тип</span><span class="sxs-lookup"><span data-stu-id="844c2-113">Type</span></span>   |<span data-ttu-id="844c2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="844c2-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="844c2-115">id</span><span class="sxs-lookup"><span data-stu-id="844c2-115">id</span></span>|<span data-ttu-id="844c2-116">Guid</span><span class="sxs-lookup"><span data-stu-id="844c2-116">Guid</span></span>|<span data-ttu-id="844c2-117">Уникальный идентификатор для одного из экземпляров [oAuth2Permission](oauth2permission.md) или [роли приложения](approle.md) , которые предоставляет доступ к приложению ресурсов.</span><span class="sxs-lookup"><span data-stu-id="844c2-117">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="844c2-118">type</span><span class="sxs-lookup"><span data-stu-id="844c2-118">type</span></span>|<span data-ttu-id="844c2-119">Строка</span><span class="sxs-lookup"><span data-stu-id="844c2-119">String</span></span>|<span data-ttu-id="844c2-120">Указывает, будет ли свойство **id** ссылается на [oAuth2Permission](oauth2permission.md) или [роли приложения](approle.md).</span><span class="sxs-lookup"><span data-stu-id="844c2-120">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="844c2-121">Возможные значения: «область» или «роли».</span><span class="sxs-lookup"><span data-stu-id="844c2-121">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
