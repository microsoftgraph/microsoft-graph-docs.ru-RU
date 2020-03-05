---
title: Тип ресурса preAuthorizedApplication
description: Список предварительно авторизованных клиентских приложений
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 69ff3d775d4cf3aa767e5e226e688334fcc9f542
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447082"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="bbd2e-103">Тип ресурса preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="bbd2e-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="bbd2e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bbd2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bbd2e-105">Перечисляет клиентские приложения, которые предварительно авторизованы с указанными разрешениями для доступа к API этого приложения.</span><span class="sxs-lookup"><span data-stu-id="bbd2e-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="bbd2e-106">Пользователям не требуется согласие с какими-либо из предварительно разрешенных приложений (для указанных разрешений).</span><span class="sxs-lookup"><span data-stu-id="bbd2e-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="bbd2e-107">Однако все дополнительные разрешения, не указанные в Преаусоризедаппликатионс (например, по запросу добавочного согласия), требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="bbd2e-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="bbd2e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbd2e-108">Properties</span></span>

| <span data-ttu-id="bbd2e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbd2e-109">Property</span></span> | <span data-ttu-id="bbd2e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bbd2e-110">Type</span></span> | <span data-ttu-id="bbd2e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd2e-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bbd2e-112">appId</span><span class="sxs-lookup"><span data-stu-id="bbd2e-112">appId</span></span>|<span data-ttu-id="bbd2e-113">String</span><span class="sxs-lookup"><span data-stu-id="bbd2e-113">String</span></span>| <span data-ttu-id="bbd2e-114">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="bbd2e-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="bbd2e-115">делегатедпермиссионидс</span><span class="sxs-lookup"><span data-stu-id="bbd2e-115">delegatedPermissionIds</span></span>|<span data-ttu-id="bbd2e-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bbd2e-116">String collection</span></span>| <span data-ttu-id="bbd2e-117">Уникальный идентификатор для [oauth2PermissionScopes](permissionscope.md) , который требуется приложению.</span><span class="sxs-lookup"><span data-stu-id="bbd2e-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bbd2e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbd2e-118">JSON representation</span></span>
<span data-ttu-id="bbd2e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbd2e-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "delegatedPermissionIds": ["String"]
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
