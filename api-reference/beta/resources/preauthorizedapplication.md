---
title: Тип ресурса preAuthorizedApplication
description: Список предварительно авторизованных клиентских приложений
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c741c303ee9ffaf18db5fc01181702f963e39ccc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939784"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="6f563-103">Тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="6f563-103">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f563-104">Перечисляет клиентские приложения, которые предварительно авторизованы с указанными разрешениями для доступа к API этого приложения.</span><span class="sxs-lookup"><span data-stu-id="6f563-104">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="6f563-105">Пользователям не требуется согласие с какими-либо из предварительно разрешенных приложений (для указанных разрешений).</span><span class="sxs-lookup"><span data-stu-id="6f563-105">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="6f563-106">Однако все дополнительные разрешения, не указанные в Преаусоризедаппликатионс (например, по запросу добавочного согласия), требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f563-106">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="6f563-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f563-107">Properties</span></span>

| <span data-ttu-id="6f563-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f563-108">Property</span></span> | <span data-ttu-id="6f563-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6f563-109">Type</span></span> | <span data-ttu-id="6f563-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f563-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6f563-111">appId</span><span class="sxs-lookup"><span data-stu-id="6f563-111">appId</span></span>|<span data-ttu-id="6f563-112">String</span><span class="sxs-lookup"><span data-stu-id="6f563-112">String</span></span>| <span data-ttu-id="6f563-113">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="6f563-113">The unique identifier for the application.</span></span> |
|<span data-ttu-id="6f563-114">пермиссионидс</span><span class="sxs-lookup"><span data-stu-id="6f563-114">permissionIds</span></span>|<span data-ttu-id="6f563-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6f563-115">String collection</span></span>| <span data-ttu-id="6f563-116">Уникальный идентификатор для [oauth2PermissionScopes](permissionscope.md) , который требуется приложению.</span><span class="sxs-lookup"><span data-stu-id="6f563-116">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f563-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f563-117">JSON representation</span></span>
<span data-ttu-id="6f563-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f563-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
