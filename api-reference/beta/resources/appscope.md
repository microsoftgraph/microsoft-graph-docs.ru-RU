---
title: Тип ресурса Аппскопе
description: Область приложения — это область, определенная и понятная определенному приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 23a3d18a8a712ddff8470d91a677f3d0f18dabf2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459337"
---
# <a name="appscope-resource-type"></a><span data-ttu-id="e0177-103">Тип ресурса Аппскопе</span><span class="sxs-lookup"><span data-stu-id="e0177-103">appScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0177-104">Область назначения роли определяет набор ресурсов, доступ к которым предоставлен участнику.</span><span class="sxs-lookup"><span data-stu-id="e0177-104">The scope of a role assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="e0177-105">Область приложения — это область, определенная и понятная определенному приложению.</span><span class="sxs-lookup"><span data-stu-id="e0177-105">An app scope is a scope defined and understood by a specific application.</span></span> <span data-ttu-id="e0177-106">Другой тип области — область действия каталога.</span><span class="sxs-lookup"><span data-stu-id="e0177-106">The other type of scope is directory scope.</span></span> <span data-ttu-id="e0177-107">Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="e0177-107">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> 

<span data-ttu-id="e0177-108">Он используется как для одного участника, так и для одной однообъектной области, так и для нескольких субъектов.</span><span class="sxs-lookup"><span data-stu-id="e0177-108">This is employed in both the single principal, single scope entity and multiple principal, multiple scope entities.</span></span>

## <a name="methods"></a><span data-ttu-id="e0177-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e0177-109">Methods</span></span>
<span data-ttu-id="e0177-110">Нет</span><span class="sxs-lookup"><span data-stu-id="e0177-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="e0177-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0177-111">Properties</span></span>

| <span data-ttu-id="e0177-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0177-112">Property</span></span> | <span data-ttu-id="e0177-113">Тип</span><span class="sxs-lookup"><span data-stu-id="e0177-113">Type</span></span> | <span data-ttu-id="e0177-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e0177-114">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e0177-115">id</span><span class="sxs-lookup"><span data-stu-id="e0177-115">id</span></span> | <span data-ttu-id="e0177-116">string</span><span class="sxs-lookup"><span data-stu-id="e0177-116">string</span></span> | <span data-ttu-id="e0177-117">Идентификатор контейнера или ресурса конкретного приложения, представляющие область назначения.</span><span class="sxs-lookup"><span data-stu-id="e0177-117">Id of an app-specific container or resource representing the scope of the assignment.</span></span> <span data-ttu-id="e0177-118">Обычно это неизменяемый идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0177-118">Usually the immutable id of the resource.</span></span> <span data-ttu-id="e0177-119">Область назначения определяет набор ресурсов, доступ к которым предоставлен участнику.</span><span class="sxs-lookup"><span data-stu-id="e0177-119">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="e0177-120">Это свойство является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e0177-120">This property is required.</span></span> |
| <span data-ttu-id="e0177-121">type</span><span class="sxs-lookup"><span data-stu-id="e0177-121">type</span></span> | <span data-ttu-id="e0177-122">String</span><span class="sxs-lookup"><span data-stu-id="e0177-122">String</span></span> | <span data-ttu-id="e0177-123">Описывает тип ресурса для конкретного приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="e0177-123">Describes the type of app-specific resource represented by the app scope.</span></span> <span data-ttu-id="e0177-124">Позволяет пользовательскому интерфейсу передать пользователю тип ресурса приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="e0177-124">Provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.</span></span> <span data-ttu-id="e0177-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0177-125">This property is read only.</span></span> |
| <span data-ttu-id="e0177-126">displayName</span><span class="sxs-lookup"><span data-stu-id="e0177-126">displayName</span></span> | <span data-ttu-id="e0177-127">string</span><span class="sxs-lookup"><span data-stu-id="e0177-127">string</span></span> | <span data-ttu-id="e0177-128">Предоставляет отображаемое имя ресурса для конкретного приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="e0177-128">Provides the display name of the app-specific resource represented by the app scope.</span></span> <span data-ttu-id="e0177-129">Используется для отображения в целях отображения, так как Аппскопеид часто является неизменяемым идентификатором, не предназначенным для человека. Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0177-129">Provided for display purposes since appScopeId is often an immutable, non-human-readable id. This property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e0177-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="e0177-130">Relationships</span></span>

<span data-ttu-id="e0177-131">Нет</span><span class="sxs-lookup"><span data-stu-id="e0177-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0177-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0177-132">JSON representation</span></span>

<span data-ttu-id="e0177-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0177-133">The following is a JSON representation of the resource.</span></span>

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