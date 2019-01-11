---
title: Тип ресурса governancePermission
description: 'Представляет, governanceSubject имеет разрешение на доступ к определенным governanceResource.  '
localization_priority: Normal
ms.openlocfilehash: e082ca50e5642e865b3e30859eea607df63a03b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882875"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="2a4ab-103">Тип ресурса governancePermission</span><span class="sxs-lookup"><span data-stu-id="2a4ab-103">governancePermission resource type</span></span>

> <span data-ttu-id="2a4ab-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2a4ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a4ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a4ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a4ab-106">Представляет, [governanceSubject](../resources/governancesubject.md) имеет разрешение на доступ к определенным [governanceResource](../resources/governanceresource.md).</span><span class="sxs-lookup"><span data-stu-id="2a4ab-106">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="2a4ab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a4ab-107">Properties</span></span>
| <span data-ttu-id="2a4ab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a4ab-108">Property</span></span>     | <span data-ttu-id="2a4ab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2a4ab-109">Type</span></span>   |<span data-ttu-id="2a4ab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2a4ab-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a4ab-111">accessLevel</span><span class="sxs-lookup"><span data-stu-id="2a4ab-111">accessLevel</span></span>|<span data-ttu-id="2a4ab-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2a4ab-112">String</span></span>|<span data-ttu-id="2a4ab-113">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="2a4ab-113">The access level.</span></span> <span data-ttu-id="2a4ab-114">Допустимые значения: ``None``, ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="2a4ab-114">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="2a4ab-115">isActive</span><span class="sxs-lookup"><span data-stu-id="2a4ab-115">isActive</span></span>|<span data-ttu-id="2a4ab-116">Логический</span><span class="sxs-lookup"><span data-stu-id="2a4ab-116">Boolean</span></span>|<span data-ttu-id="2a4ab-117">Указывает, если инициатора запроса имеет назначения активная роль на уровне доступа.</span><span class="sxs-lookup"><span data-stu-id="2a4ab-117">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="2a4ab-118">isEligible</span><span class="sxs-lookup"><span data-stu-id="2a4ab-118">isEligible</span></span>|<span data-ttu-id="2a4ab-119">Логический</span><span class="sxs-lookup"><span data-stu-id="2a4ab-119">Boolean</span></span>|<span data-ttu-id="2a4ab-120">Указывает, имеет ли инициатора запроса все назначения ролей право на уровне доступа.</span><span class="sxs-lookup"><span data-stu-id="2a4ab-120">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a4ab-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a4ab-121">JSON representation</span></span>

<span data-ttu-id="2a4ab-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a4ab-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
