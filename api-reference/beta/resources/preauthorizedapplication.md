---
title: тип ресурса preAuthorizedApplication
description: Списки предварительно авторизованных клиентских приложений
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 94a8dad23492ca7a145c5839410edf0fd4a34877
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761165"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="8a95f-103">тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="8a95f-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="8a95f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a95f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a95f-105">Перечислены клиентские приложения, предварительно авторизованные с указанными разрешениями на доступ к API этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8a95f-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="8a95f-106">Пользователи не обязаны соглашаться на любое предварительно авторизованного приложения (для указанных разрешений).</span><span class="sxs-lookup"><span data-stu-id="8a95f-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="8a95f-107">Однако для любых дополнительных разрешений, не указанных в preAuthorizedApplications (запрашивается, например, с помощью дополнительного согласия), потребуется согласие пользователя.</span><span class="sxs-lookup"><span data-stu-id="8a95f-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="8a95f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a95f-108">Properties</span></span>

| <span data-ttu-id="8a95f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a95f-109">Property</span></span> | <span data-ttu-id="8a95f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8a95f-110">Type</span></span> | <span data-ttu-id="8a95f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8a95f-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8a95f-112">appId</span><span class="sxs-lookup"><span data-stu-id="8a95f-112">appId</span></span>|<span data-ttu-id="8a95f-113">String</span><span class="sxs-lookup"><span data-stu-id="8a95f-113">String</span></span>| <span data-ttu-id="8a95f-114">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="8a95f-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="8a95f-115">permissionIds</span><span class="sxs-lookup"><span data-stu-id="8a95f-115">permissionIds</span></span>|<span data-ttu-id="8a95f-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8a95f-116">String collection</span></span>| <span data-ttu-id="8a95f-117">Уникальный идентификатор [oauth2PermissionScopes,](permissionscope.md) который требуется приложению.</span><span class="sxs-lookup"><span data-stu-id="8a95f-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8a95f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a95f-118">JSON representation</span></span>
<span data-ttu-id="8a95f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a95f-119">Here is a JSON representation of the resource.</span></span>

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


