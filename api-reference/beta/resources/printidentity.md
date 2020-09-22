---
title: Тип ресурса Принтидентити
description: Представляет удостоверение в универсальной службе печати. Сопоставление группы Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 45a69cbad25d2f9c3c99c9e01aa47982fe5c62b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048773"
---
# <a name="printidentity-resource-type"></a><span data-ttu-id="8adf1-104">Тип ресурса Принтидентити</span><span class="sxs-lookup"><span data-stu-id="8adf1-104">printIdentity resource type</span></span>

<span data-ttu-id="8adf1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8adf1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8adf1-106">Представляет удостоверение в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="8adf1-106">Represents an identity within the Universal Print service.</span></span> <span data-ttu-id="8adf1-107">Сопоставление с [группой Azure Active Directory (Azure AD)](group.md).</span><span class="sxs-lookup"><span data-stu-id="8adf1-107">Maps to an [Azure Active Directory (Azure AD) group](group.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8adf1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8adf1-108">Properties</span></span>
| <span data-ttu-id="8adf1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8adf1-109">Property</span></span>     | <span data-ttu-id="8adf1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8adf1-110">Type</span></span>        | <span data-ttu-id="8adf1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8adf1-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8adf1-112">id</span><span class="sxs-lookup"><span data-stu-id="8adf1-112">id</span></span>|<span data-ttu-id="8adf1-113">Строка</span><span class="sxs-lookup"><span data-stu-id="8adf1-113">String</span></span>|<span data-ttu-id="8adf1-114">Идентификатор Принтидентити.</span><span class="sxs-lookup"><span data-stu-id="8adf1-114">The printIdentity's identifier.</span></span> <span data-ttu-id="8adf1-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8adf1-115">Read-only.</span></span>|
|<span data-ttu-id="8adf1-116">displayName</span><span class="sxs-lookup"><span data-stu-id="8adf1-116">displayName</span></span>|<span data-ttu-id="8adf1-117">Строка</span><span class="sxs-lookup"><span data-stu-id="8adf1-117">String</span></span>|<span data-ttu-id="8adf1-118">Отображаемое имя Принтидентити.</span><span class="sxs-lookup"><span data-stu-id="8adf1-118">The printIdentity's display name.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8adf1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8adf1-119">JSON representation</span></span>

<span data-ttu-id="8adf1-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8adf1-120">The following is a JSON representation of the resource.</span></span>

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


