---
title: Тип ресурса Провисионедидентити
description: Описывает удостоверение, связанное со сводным событием объекта наполнения.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5fde45d8e9baf28fddfe9935d71689d24059dfa3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371397"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="97334-103">Тип ресурса Провисионедидентити</span><span class="sxs-lookup"><span data-stu-id="97334-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="97334-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97334-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97334-105">Описывает удостоверение, связанное со сводным событием объекта наполнения.</span><span class="sxs-lookup"><span data-stu-id="97334-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="97334-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="97334-106">Properties</span></span>

| <span data-ttu-id="97334-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="97334-107">Property</span></span>     | <span data-ttu-id="97334-108">Тип</span><span class="sxs-lookup"><span data-stu-id="97334-108">Type</span></span>        | <span data-ttu-id="97334-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97334-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97334-110">details</span><span class="sxs-lookup"><span data-stu-id="97334-110">details</span></span>|[<span data-ttu-id="97334-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="97334-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="97334-112">Сведения об удостоверении.</span><span class="sxs-lookup"><span data-stu-id="97334-112">Details of the identity.</span></span>|
|<span data-ttu-id="97334-113">displayName</span><span class="sxs-lookup"><span data-stu-id="97334-113">displayName</span></span>|<span data-ttu-id="97334-114">Строка</span><span class="sxs-lookup"><span data-stu-id="97334-114">String</span></span>|<span data-ttu-id="97334-115">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="97334-115">Display name of the identity.</span></span> |
|<span data-ttu-id="97334-116">id</span><span class="sxs-lookup"><span data-stu-id="97334-116">id</span></span>|<span data-ttu-id="97334-117">String</span><span class="sxs-lookup"><span data-stu-id="97334-117">String</span></span>|<span data-ttu-id="97334-118">Уникально идентифицирует удостоверение.</span><span class="sxs-lookup"><span data-stu-id="97334-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="97334-119">идентититипе</span><span class="sxs-lookup"><span data-stu-id="97334-119">identityType</span></span>|<span data-ttu-id="97334-120">String</span><span class="sxs-lookup"><span data-stu-id="97334-120">String</span></span>|<span data-ttu-id="97334-121">Тип удостоверения, которое было подготовлено, например "пользователь" или "Группа".</span><span class="sxs-lookup"><span data-stu-id="97334-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97334-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97334-122">JSON representation</span></span>

<span data-ttu-id="97334-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97334-123">The following is a JSON representation of the resource.</span></span>

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
