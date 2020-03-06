---
title: Тип ресурса Рекуиредресаурцеакцесс
description: Задает набор областей разрешений и ролей приложений для OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 45b7e8d2598ca58ef4d78bb45c3b2a8f51955353
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533842"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="deb17-103">Тип ресурса Рекуиредресаурцеакцесс</span><span class="sxs-lookup"><span data-stu-id="deb17-103">requiredResourceAccess resource type</span></span>

<span data-ttu-id="deb17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb17-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="deb17-105">Задает набор областей разрешений OAuth 2,0 и ролей приложения в указанном ресурсе, к которому приложение требует доступ.</span><span class="sxs-lookup"><span data-stu-id="deb17-105">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="deb17-106">Указанные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** ) при вызове приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="deb17-106">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="deb17-107">Свойство **рекуиредресаурцеакцесс** объекта [Application](application.md) представляет собой коллекцию **рекиредресаурцеакцесс**.</span><span class="sxs-lookup"><span data-stu-id="deb17-107">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="deb17-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="deb17-108">JSON representation</span></span>

<span data-ttu-id="deb17-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="deb17-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="deb17-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="deb17-110">Properties</span></span>
| <span data-ttu-id="deb17-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="deb17-111">Property</span></span>     | <span data-ttu-id="deb17-112">Тип</span><span class="sxs-lookup"><span data-stu-id="deb17-112">Type</span></span>   |<span data-ttu-id="deb17-113">Описание</span><span class="sxs-lookup"><span data-stu-id="deb17-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deb17-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="deb17-114">resourceAccess</span></span>|<span data-ttu-id="deb17-115">Коллекция [ресаурцеакцесс](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="deb17-115">[resourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="deb17-116">Список областей разрешений OAuth 2.0 и ролей приложений, которые требуются приложению из указанного ресурса.</span><span class="sxs-lookup"><span data-stu-id="deb17-116">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="deb17-117">ресаурцеаппид</span><span class="sxs-lookup"><span data-stu-id="deb17-117">resourceAppId</span></span>|<span data-ttu-id="deb17-118">Строка</span><span class="sxs-lookup"><span data-stu-id="deb17-118">String</span></span>|<span data-ttu-id="deb17-119">Уникальный идентификатор ресурса, доступ к которому требуется приложению.</span><span class="sxs-lookup"><span data-stu-id="deb17-119">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="deb17-120">Он должен быть равен **AppID** , объявленному в целевом приложении ресурсов.</span><span class="sxs-lookup"><span data-stu-id="deb17-120">This should be equal to the **appId** declared on the target resource application.</span></span>|

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
