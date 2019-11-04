---
title: Тип ресурса Рекуиредресаурцеакцесс
description: Задает набор областей разрешений и ролей приложений для OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e6e6577eb6ee23ba430054b43de38fc2dd3a1904
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939795"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="1fe61-103">Тип ресурса Рекуиредресаурцеакцесс</span><span class="sxs-lookup"><span data-stu-id="1fe61-103">requiredResourceAccess resource type</span></span>

<span data-ttu-id="1fe61-104">Задает набор областей разрешений OAuth 2,0 и ролей приложения в указанном ресурсе, к которому приложение требует доступ.</span><span class="sxs-lookup"><span data-stu-id="1fe61-104">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="1fe61-105">Указанные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** ) при вызове приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="1fe61-105">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="1fe61-106">Свойство **рекуиредресаурцеакцесс** объекта [Application](application.md) представляет собой коллекцию **рекиредресаурцеакцесс**.</span><span class="sxs-lookup"><span data-stu-id="1fe61-106">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1fe61-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fe61-107">JSON representation</span></span>

<span data-ttu-id="1fe61-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="1fe61-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="1fe61-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fe61-109">Properties</span></span>
| <span data-ttu-id="1fe61-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fe61-110">Property</span></span>     | <span data-ttu-id="1fe61-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1fe61-111">Type</span></span>   |<span data-ttu-id="1fe61-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1fe61-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fe61-113">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="1fe61-113">resourceAccess</span></span>|<span data-ttu-id="1fe61-114">Коллекция [ресаурцеакцесс](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="1fe61-114">[resourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="1fe61-115">Список областей разрешений OAuth 2.0 и ролей приложений, которые требуются приложению из указанного ресурса.</span><span class="sxs-lookup"><span data-stu-id="1fe61-115">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="1fe61-116">ресаурцеаппид</span><span class="sxs-lookup"><span data-stu-id="1fe61-116">resourceAppId</span></span>|<span data-ttu-id="1fe61-117">String</span><span class="sxs-lookup"><span data-stu-id="1fe61-117">String</span></span>|<span data-ttu-id="1fe61-118">Уникальный идентификатор ресурса, доступ к которому требуется приложению.</span><span class="sxs-lookup"><span data-stu-id="1fe61-118">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="1fe61-119">Он должен быть равен **AppID** , объявленному в целевом приложении ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1fe61-119">This should be equal to the **appId** declared on the target resource application.</span></span>|

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
