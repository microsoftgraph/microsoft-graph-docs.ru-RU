---
title: Тип ресурса Азуреактиведиректоритенант
description: Тип Азуреактиведиректоритенант определяет другого клиента Azure Active Directory в качестве источника удостоверения для подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 881454f9658ae266705804518c3b5d8a876861eb
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510356"
---
# <a name="azureactivedirectorytenant-resource-type"></a><span data-ttu-id="b4b38-103">Тип ресурса Азуреактиведиректоритенант</span><span class="sxs-lookup"><span data-stu-id="b4b38-103">azureActiveDirectoryTenant resource type</span></span>

<span data-ttu-id="b4b38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4b38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4b38-105">Используется в источниках удостоверений [коннектедорганизатион](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="b4b38-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="b4b38-106">`@odata.type`Значение `#microsoft.graph.azureActiveDirectoryTenant` указывает на то, что этот тип определяет другого клиента Azure Active Directory в качестве источника удостоверений для подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="b4b38-106">The `@odata.type` value `#microsoft.graph.azureActiveDirectoryTenant` indicates that this type identifies another Azure Active Directory tenant as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="b4b38-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4b38-107">Properties</span></span>

| <span data-ttu-id="b4b38-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4b38-108">Property</span></span>                     | <span data-ttu-id="b4b38-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b4b38-109">Type</span></span>                      | <span data-ttu-id="b4b38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b4b38-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="b4b38-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b4b38-111">displayName</span></span> |<span data-ttu-id="b4b38-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b4b38-112">String</span></span> | <span data-ttu-id="b4b38-113">Имя клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b4b38-113">The name of the Azure Active Directory tenant.</span></span> <span data-ttu-id="b4b38-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4b38-114">Read only.</span></span> |
| <span data-ttu-id="b4b38-115">tenantId</span><span class="sxs-lookup"><span data-stu-id="b4b38-115">tenantId</span></span> |<span data-ttu-id="b4b38-116">String</span><span class="sxs-lookup"><span data-stu-id="b4b38-116">String</span></span> | <span data-ttu-id="b4b38-117">Идентификатор клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b4b38-117">The ID of the Azure Active Directory tenant.</span></span> <span data-ttu-id="b4b38-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4b38-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b4b38-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b4b38-119">Relationships</span></span>

<span data-ttu-id="b4b38-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b4b38-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4b38-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b4b38-121">JSON representation</span></span>

<span data-ttu-id="b4b38-122">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4b38-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "azureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
