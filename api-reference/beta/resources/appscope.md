---
title: Тип ресурса Аппскопе
description: 'Область назначения роли определяет набор ресурсов, доступ к которым предоставлен участнику. Область приложения — это область, определенная и понятная определенному приложению. Другой тип области — область действия каталога. Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a996b219df124ac0c287ed4ed32658584acb6ac
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160426"
---
# <a name="appscope-resource-type"></a><span data-ttu-id="49b0a-106">Тип ресурса Аппскопе</span><span class="sxs-lookup"><span data-stu-id="49b0a-106">appScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49b0a-107">Область назначения роли определяет набор ресурсов, доступ к которым предоставлен участнику.</span><span class="sxs-lookup"><span data-stu-id="49b0a-107">The scope of a role assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="49b0a-108">Область приложения — это область, определенная и понятная определенному приложению.</span><span class="sxs-lookup"><span data-stu-id="49b0a-108">An app scope is a scope defined and understood by a specific application.</span></span> <span data-ttu-id="49b0a-109">Другой тип области — область действия каталога.</span><span class="sxs-lookup"><span data-stu-id="49b0a-109">The other type of scope is directory scope.</span></span> <span data-ttu-id="49b0a-110">Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="49b0a-110">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> 

<span data-ttu-id="49b0a-111">Он используется как для одного участника, так и для одной однообъектной области, так и для нескольких субъектов.</span><span class="sxs-lookup"><span data-stu-id="49b0a-111">This is employed in both the single principal, single scope entity and multiple principal, multiple scope entities.</span></span>

## <a name="methods"></a><span data-ttu-id="49b0a-112">Методы</span><span class="sxs-lookup"><span data-stu-id="49b0a-112">Methods</span></span>
<span data-ttu-id="49b0a-113">Нет</span><span class="sxs-lookup"><span data-stu-id="49b0a-113">None</span></span>

## <a name="properties"></a><span data-ttu-id="49b0a-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="49b0a-114">Properties</span></span>

| <span data-ttu-id="49b0a-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="49b0a-115">Property</span></span> | <span data-ttu-id="49b0a-116">Тип</span><span class="sxs-lookup"><span data-stu-id="49b0a-116">Type</span></span> | <span data-ttu-id="49b0a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="49b0a-117">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="49b0a-118">id</span><span class="sxs-lookup"><span data-stu-id="49b0a-118">id</span></span> | <span data-ttu-id="49b0a-119">string</span><span class="sxs-lookup"><span data-stu-id="49b0a-119">string</span></span> | <span data-ttu-id="49b0a-120">Идентификатор контейнера или ресурса конкретного приложения, представляющие область назначения.</span><span class="sxs-lookup"><span data-stu-id="49b0a-120">Id of an app-specific container or resource representing the scope of the assignment.</span></span> <span data-ttu-id="49b0a-121">Обычно это неизменяемый идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="49b0a-121">Usually the immutable id of the resource.</span></span> <span data-ttu-id="49b0a-122">Область назначения определяет набор ресурсов, доступ к которым предоставлен участнику.</span><span class="sxs-lookup"><span data-stu-id="49b0a-122">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="49b0a-123">Это свойство является обязательным.</span><span class="sxs-lookup"><span data-stu-id="49b0a-123">This property is required.</span></span> |
| <span data-ttu-id="49b0a-124">type</span><span class="sxs-lookup"><span data-stu-id="49b0a-124">type</span></span> | <span data-ttu-id="49b0a-125">String</span><span class="sxs-lookup"><span data-stu-id="49b0a-125">String</span></span> | <span data-ttu-id="49b0a-126">Описывает тип ресурса для конкретного приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="49b0a-126">Describes the type of app-specific resource represented by the app scope.</span></span> <span data-ttu-id="49b0a-127">Позволяет пользовательскому интерфейсу передать пользователю тип ресурса приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="49b0a-127">Provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.</span></span> <span data-ttu-id="49b0a-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49b0a-128">This property is read only.</span></span> |
| <span data-ttu-id="49b0a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="49b0a-129">displayName</span></span> | <span data-ttu-id="49b0a-130">string</span><span class="sxs-lookup"><span data-stu-id="49b0a-130">string</span></span> | <span data-ttu-id="49b0a-131">Предоставляет отображаемое имя ресурса для конкретного приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="49b0a-131">Provides the display name of the app-specific resource represented by the app scope.</span></span> <span data-ttu-id="49b0a-132">Используется для отображения в целях отображения, так как Аппскопеид часто является неизменяемым идентификатором, не предназначенным для человека. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49b0a-132">Provided for display purposes since appScopeId is often an immutable, non-human-readable id. This property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="49b0a-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="49b0a-133">Relationships</span></span>

<span data-ttu-id="49b0a-134">Нет</span><span class="sxs-lookup"><span data-stu-id="49b0a-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49b0a-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49b0a-135">JSON representation</span></span>

<span data-ttu-id="49b0a-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49b0a-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appScope"
}-->

```json
{
  "id": "String (identifier)",
  "type": "String",
  "displayName": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->