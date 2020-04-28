---
title: Тип ресурса Принтидентити
description: Представляет удостоверение в универсальной службе печати. Сопоставление группы Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d4ac0695357aba0ba6c44fef4654d2edaefca6cb
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917612"
---
# <a name="printidentity-resource-type"></a><span data-ttu-id="056c3-104">Тип ресурса Принтидентити</span><span class="sxs-lookup"><span data-stu-id="056c3-104">printIdentity resource type</span></span>

<span data-ttu-id="056c3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="056c3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="056c3-106">Представляет удостоверение в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="056c3-106">Represents an identity within the Universal Print service.</span></span> <span data-ttu-id="056c3-107">Сопоставление с [группой Azure Active Directory (Azure AD)](group.md).</span><span class="sxs-lookup"><span data-stu-id="056c3-107">Maps to an [Azure Active Directory (Azure AD) group](group.md).</span></span>

## <a name="properties"></a><span data-ttu-id="056c3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="056c3-108">Properties</span></span>
| <span data-ttu-id="056c3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="056c3-109">Property</span></span>     | <span data-ttu-id="056c3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="056c3-110">Type</span></span>        | <span data-ttu-id="056c3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="056c3-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="056c3-112">id</span><span class="sxs-lookup"><span data-stu-id="056c3-112">id</span></span>|<span data-ttu-id="056c3-113">String</span><span class="sxs-lookup"><span data-stu-id="056c3-113">String</span></span>|<span data-ttu-id="056c3-114">Идентификатор Принтидентити.</span><span class="sxs-lookup"><span data-stu-id="056c3-114">The printIdentity's identifier.</span></span> <span data-ttu-id="056c3-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="056c3-115">Read-only.</span></span>|
|<span data-ttu-id="056c3-116">displayName</span><span class="sxs-lookup"><span data-stu-id="056c3-116">displayName</span></span>|<span data-ttu-id="056c3-117">Строка</span><span class="sxs-lookup"><span data-stu-id="056c3-117">String</span></span>|<span data-ttu-id="056c3-118">Отображаемое имя Принтидентити.</span><span class="sxs-lookup"><span data-stu-id="056c3-118">The printIdentity's display name.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="056c3-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="056c3-119">JSON representation</span></span>

<span data-ttu-id="056c3-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="056c3-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
