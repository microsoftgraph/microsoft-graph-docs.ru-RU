---
title: Тип ресурса requiredResourceAccess
description: Указывает набор областей разрешений OAuth 2.0 и ролей приложений.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: f9a847e6863353e59602aef3c794bc7d79e40d5e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133723"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="021eb-103">Тип ресурса requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="021eb-103">requiredResourceAccess resource type</span></span>

<span data-ttu-id="021eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="021eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="021eb-105">Указывает набор областей разрешений OAuth 2.0 и ролей приложения в указанном ресурсе, к который приложению требуется доступ.</span><span class="sxs-lookup"><span data-stu-id="021eb-105">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="021eb-106">Указанные области разрешений OAuth 2.0 могут запрашиваться клиентских приложений (с помощью коллекции **requiredResourceAccess)** при вызове приложения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="021eb-106">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="021eb-107">Свойство **requiredResourceAccess** объекта [приложения](application.md) — это коллекция **Re.redResourceAccess.**</span><span class="sxs-lookup"><span data-stu-id="021eb-107">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="021eb-108">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="021eb-108">JSON representation</span></span>

<span data-ttu-id="021eb-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="021eb-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a><span data-ttu-id="021eb-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="021eb-110">Properties</span></span>
| <span data-ttu-id="021eb-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="021eb-111">Property</span></span>     | <span data-ttu-id="021eb-112">Тип</span><span class="sxs-lookup"><span data-stu-id="021eb-112">Type</span></span>   |<span data-ttu-id="021eb-113">Описание</span><span class="sxs-lookup"><span data-stu-id="021eb-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="021eb-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="021eb-114">resourceAccess</span></span>|<span data-ttu-id="021eb-115">[Коллекция ResourceAccess](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="021eb-115">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="021eb-116">Список областей разрешений OAuth2.0 и ролей приложений, необходимых приложению для указанного ресурса.</span><span class="sxs-lookup"><span data-stu-id="021eb-116">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="021eb-117">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="021eb-117">resourceAppId</span></span>|<span data-ttu-id="021eb-118">Строка</span><span class="sxs-lookup"><span data-stu-id="021eb-118">String</span></span>|<span data-ttu-id="021eb-119">Уникальный идентификатор ресурса, к котором приложению требуется доступ.</span><span class="sxs-lookup"><span data-stu-id="021eb-119">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="021eb-120">Он должен быть равен **appId, объявленным** в целевом приложении ресурсов.</span><span class="sxs-lookup"><span data-stu-id="021eb-120">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


