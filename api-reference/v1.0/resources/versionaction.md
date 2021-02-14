---
author: daspek
title: Тип ресурса versionAction
description: Объект VersionAction предоставляет сведения о действии, которое привело к новой версии элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f47d90c899ea9eb011837ae3c47dd6ec7ae22f30
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238990"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="63a2a-103">Тип ресурса versionAction</span><span class="sxs-lookup"><span data-stu-id="63a2a-103">versionAction resource type</span></span>

<span data-ttu-id="63a2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a2a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63a2a-105">Наличие ресурса **versionAction** в [**itemActivity**][activity] указывает на то, что действие вызвало новую версию для создания.</span><span class="sxs-lookup"><span data-stu-id="63a2a-105">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="63a2a-106">**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="63a2a-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="63a2a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="63a2a-107">Properties</span></span>

| <span data-ttu-id="63a2a-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="63a2a-108">Property name</span></span> | <span data-ttu-id="63a2a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="63a2a-109">Type</span></span>   | <span data-ttu-id="63a2a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="63a2a-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="63a2a-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="63a2a-111">newVersion</span></span>    | <span data-ttu-id="63a2a-112">string</span><span class="sxs-lookup"><span data-stu-id="63a2a-112">string</span></span> | <span data-ttu-id="63a2a-113">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="63a2a-113">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63a2a-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63a2a-114">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->

