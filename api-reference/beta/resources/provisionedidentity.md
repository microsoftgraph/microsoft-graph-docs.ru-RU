---
title: Тип ресурса Провисионедидентити
description: Описывает удостоверение, связанное со сводным событием объекта наполнения.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb535bbba827f93b597c5e41efb128f2ad610ef2
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349435"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="ffe86-103">Тип ресурса Провисионедидентити</span><span class="sxs-lookup"><span data-stu-id="ffe86-103">provisionedIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffe86-104">Описывает удостоверение, связанное со сводным событием объекта наполнения.</span><span class="sxs-lookup"><span data-stu-id="ffe86-104">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="ffe86-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffe86-105">Properties</span></span>

| <span data-ttu-id="ffe86-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffe86-106">Property</span></span>     | <span data-ttu-id="ffe86-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ffe86-107">Type</span></span>        | <span data-ttu-id="ffe86-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ffe86-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ffe86-109">details</span><span class="sxs-lookup"><span data-stu-id="ffe86-109">details</span></span>|[<span data-ttu-id="ffe86-110">Детаилсинфо</span><span class="sxs-lookup"><span data-stu-id="ffe86-110">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="ffe86-111">Сведения об удостоверении.</span><span class="sxs-lookup"><span data-stu-id="ffe86-111">Details of the identity.</span></span>|
|<span data-ttu-id="ffe86-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ffe86-112">displayName</span></span>|<span data-ttu-id="ffe86-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ffe86-113">String</span></span>|<span data-ttu-id="ffe86-114">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ffe86-114">Display name of the identity.</span></span> |
|<span data-ttu-id="ffe86-115">id</span><span class="sxs-lookup"><span data-stu-id="ffe86-115">id</span></span>|<span data-ttu-id="ffe86-116">String</span><span class="sxs-lookup"><span data-stu-id="ffe86-116">String</span></span>|<span data-ttu-id="ffe86-117">Уникально идентифицирует удостоверение.</span><span class="sxs-lookup"><span data-stu-id="ffe86-117">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="ffe86-118">Идентититипе</span><span class="sxs-lookup"><span data-stu-id="ffe86-118">identityType</span></span>|<span data-ttu-id="ffe86-119">String</span><span class="sxs-lookup"><span data-stu-id="ffe86-119">String</span></span>|<span data-ttu-id="ffe86-120">Тип удостоверения, которое было подготовлено, например "пользователь" или "Группа".</span><span class="sxs-lookup"><span data-stu-id="ffe86-120">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffe86-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffe86-121">JSON representation</span></span>

<span data-ttu-id="ffe86-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffe86-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
