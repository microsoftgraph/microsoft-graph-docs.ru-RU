---
title: сложный тип Коннектедорганизатионмемберс
description: Тип Коннектедорганизатионмемберс определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f2a3b55e3fab41f0fe08fcf844a6d143b12d7146
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331479"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="66e28-103">сложный тип Коннектедорганизатионмемберс</span><span class="sxs-lookup"><span data-stu-id="66e28-103">connectedOrganizationMembers complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66e28-104">Используется в параметрах запроса [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="66e28-104">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="66e28-105">`@odata.type` Значение `#microsoft.graph.connectedOrganizationMembers` указывает на то, что этот тип определяет коллекцию пользователей, которые связаны с подключенной Организацией и могут запрашивать пакет Access.</span><span class="sxs-lookup"><span data-stu-id="66e28-105">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a connected organization, who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="66e28-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="66e28-106">Properties</span></span>

<span data-ttu-id="66e28-107">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="66e28-107">This type has the following properties:</span></span>

| <span data-ttu-id="66e28-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="66e28-108">Property</span></span>                     | <span data-ttu-id="66e28-109">Тип</span><span class="sxs-lookup"><span data-stu-id="66e28-109">Type</span></span>                      | <span data-ttu-id="66e28-110">Описание</span><span class="sxs-lookup"><span data-stu-id="66e28-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="66e28-111">id</span><span class="sxs-lookup"><span data-stu-id="66e28-111">id</span></span> |<span data-ttu-id="66e28-112">Строка</span><span class="sxs-lookup"><span data-stu-id="66e28-112">String</span></span> | <span data-ttu-id="66e28-113">Идентификатор подключенной Организации в управлении обслуживанием.</span><span class="sxs-lookup"><span data-stu-id="66e28-113">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="66e28-114">description</span><span class="sxs-lookup"><span data-stu-id="66e28-114">description</span></span> |<span data-ttu-id="66e28-115">String</span><span class="sxs-lookup"><span data-stu-id="66e28-115">String</span></span> | <span data-ttu-id="66e28-116">Имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="66e28-116">The name of the connected organization.</span></span> <span data-ttu-id="66e28-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66e28-117">Read only.</span></span> |
| <span data-ttu-id="66e28-118">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="66e28-118">isBackup</span></span> | <span data-ttu-id="66e28-119">Логический</span><span class="sxs-lookup"><span data-stu-id="66e28-119">Boolean</span></span> | <span data-ttu-id="66e28-120">Не используется в данный момент.</span><span class="sxs-lookup"><span data-stu-id="66e28-120">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66e28-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66e28-121">JSON representation</span></span>

<span data-ttu-id="66e28-122">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66e28-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
  "isBackup": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
