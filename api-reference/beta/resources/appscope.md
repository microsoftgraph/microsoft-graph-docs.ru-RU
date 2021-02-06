---
title: Тип ресурса appScope
description: Область приложения — это область, определенная и понятная определенным приложением.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: de49425bddc5905d1b1bf17afeb5fb7c5363038c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136019"
---
# <a name="appscope-resource-type"></a><span data-ttu-id="9c9ee-103">Тип ресурса appScope</span><span class="sxs-lookup"><span data-stu-id="9c9ee-103">appScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c9ee-104">Область назначения роли определяет набор ресурсов, к которым был предоставлен доступ для основного.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-104">The scope of a role assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="9c9ee-105">Область приложения — это область, определенная и понятная определенным приложением.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-105">An app scope is a scope defined and understood by a specific application.</span></span> <span data-ttu-id="9c9ee-106">Другим типом области является область каталога.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-106">The other type of scope is directory scope.</span></span> <span data-ttu-id="9c9ee-107">Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-107">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> 

<span data-ttu-id="9c9ee-108">Он используется как для одного субъекта, одной сущности области, так и для нескольких субъектов с несколькими сущностями области.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-108">This is employed in both the single principal, single scope entity and multiple principal, multiple scope entities.</span></span>

## <a name="methods"></a><span data-ttu-id="9c9ee-109">Методы</span><span class="sxs-lookup"><span data-stu-id="9c9ee-109">Methods</span></span>
<span data-ttu-id="9c9ee-110">Нет</span><span class="sxs-lookup"><span data-stu-id="9c9ee-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="9c9ee-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c9ee-111">Properties</span></span>

| <span data-ttu-id="9c9ee-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c9ee-112">Property</span></span> | <span data-ttu-id="9c9ee-113">Тип</span><span class="sxs-lookup"><span data-stu-id="9c9ee-113">Type</span></span> | <span data-ttu-id="9c9ee-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9c9ee-114">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="9c9ee-115">id</span><span class="sxs-lookup"><span data-stu-id="9c9ee-115">id</span></span> | <span data-ttu-id="9c9ee-116">string</span><span class="sxs-lookup"><span data-stu-id="9c9ee-116">string</span></span> | <span data-ttu-id="9c9ee-117">ИД контейнера или ресурса для конкретного приложения, представляющего область назначения.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-117">Id of an app-specific container or resource representing the scope of the assignment.</span></span> <span data-ttu-id="9c9ee-118">Обычно не изменяемый ид ресурса.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-118">Usually the immutable id of the resource.</span></span> <span data-ttu-id="9c9ee-119">Область назначения определяет набор ресурсов, к которым был предоставлен доступ для основного.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-119">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="9c9ee-120">Это свойство является обязательной.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-120">This property is required.</span></span> |
| <span data-ttu-id="9c9ee-121">type</span><span class="sxs-lookup"><span data-stu-id="9c9ee-121">type</span></span> | <span data-ttu-id="9c9ee-122">Строка</span><span class="sxs-lookup"><span data-stu-id="9c9ee-122">String</span></span> | <span data-ttu-id="9c9ee-123">Описывает тип ресурса для конкретного приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-123">Describes the type of app-specific resource represented by the app scope.</span></span> <span data-ttu-id="9c9ee-124">Предоставляется для отображения, чтобы пользовательский интерфейс передавал пользователю тип ресурса приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-124">Provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.</span></span> <span data-ttu-id="9c9ee-125">Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-125">This property is read only.</span></span> |
| <span data-ttu-id="9c9ee-126">displayName</span><span class="sxs-lookup"><span data-stu-id="9c9ee-126">displayName</span></span> | <span data-ttu-id="9c9ee-127">string</span><span class="sxs-lookup"><span data-stu-id="9c9ee-127">string</span></span> | <span data-ttu-id="9c9ee-128">Отображает имя ресурса для конкретного приложения, представленного областью приложения.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-128">Provides the display name of the app-specific resource represented by the app scope.</span></span> <span data-ttu-id="9c9ee-129">Предоставляется для отображения, так как appScopeId часто является неусвояемым, нечитаемым для чтения ид. Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-129">Provided for display purposes since appScopeId is often an immutable, non-human-readable id. This property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9c9ee-130">Связи</span><span class="sxs-lookup"><span data-stu-id="9c9ee-130">Relationships</span></span>

<span data-ttu-id="9c9ee-131">Нет</span><span class="sxs-lookup"><span data-stu-id="9c9ee-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c9ee-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c9ee-132">JSON representation</span></span>

<span data-ttu-id="9c9ee-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c9ee-133">The following is a JSON representation of the resource.</span></span>

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

