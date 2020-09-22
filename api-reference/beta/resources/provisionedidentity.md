---
title: Тип ресурса Провисионедидентити
description: Описывает удостоверение, связанное со сводным событием объекта наполнения.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03270c0b5e6ea373ad87355612ddfb85b428d61c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993142"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="2d1cc-103">Тип ресурса Провисионедидентити</span><span class="sxs-lookup"><span data-stu-id="2d1cc-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="2d1cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d1cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d1cc-105">Описывает удостоверение, связанное со сводным событием объекта наполнения.</span><span class="sxs-lookup"><span data-stu-id="2d1cc-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="2d1cc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d1cc-106">Properties</span></span>

| <span data-ttu-id="2d1cc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d1cc-107">Property</span></span>     | <span data-ttu-id="2d1cc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2d1cc-108">Type</span></span>        | <span data-ttu-id="2d1cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2d1cc-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d1cc-110">details</span><span class="sxs-lookup"><span data-stu-id="2d1cc-110">details</span></span>|[<span data-ttu-id="2d1cc-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="2d1cc-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="2d1cc-112">Сведения об удостоверении.</span><span class="sxs-lookup"><span data-stu-id="2d1cc-112">Details of the identity.</span></span>|
|<span data-ttu-id="2d1cc-113">displayName</span><span class="sxs-lookup"><span data-stu-id="2d1cc-113">displayName</span></span>|<span data-ttu-id="2d1cc-114">String</span><span class="sxs-lookup"><span data-stu-id="2d1cc-114">String</span></span>|<span data-ttu-id="2d1cc-115">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2d1cc-115">Display name of the identity.</span></span> |
|<span data-ttu-id="2d1cc-116">id</span><span class="sxs-lookup"><span data-stu-id="2d1cc-116">id</span></span>|<span data-ttu-id="2d1cc-117">String</span><span class="sxs-lookup"><span data-stu-id="2d1cc-117">String</span></span>|<span data-ttu-id="2d1cc-118">Уникально идентифицирует удостоверение.</span><span class="sxs-lookup"><span data-stu-id="2d1cc-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="2d1cc-119">идентититипе</span><span class="sxs-lookup"><span data-stu-id="2d1cc-119">identityType</span></span>|<span data-ttu-id="2d1cc-120">String</span><span class="sxs-lookup"><span data-stu-id="2d1cc-120">String</span></span>|<span data-ttu-id="2d1cc-121">Тип удостоверения, которое было подготовлено, например "пользователь" или "Группа".</span><span class="sxs-lookup"><span data-stu-id="2d1cc-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d1cc-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d1cc-122">JSON representation</span></span>

<span data-ttu-id="2d1cc-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d1cc-123">The following is a JSON representation of the resource.</span></span>

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


