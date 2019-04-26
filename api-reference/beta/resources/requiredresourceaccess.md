---
title: Тип ресурса Рекуиредресаурцеакцесс
description: Задает набор областей разрешений OAuth 2,0 и ролей приложения в указанном ресурсе, к которому приложение требует доступ. Указанные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** ) при вызове приложения-ресурса. Свойство **рекуиредресаурцеакцесс** объекта Application представляет собой коллекцию **рекиредресаурцеакцесс**.
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563182"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="d73ca-105">Тип ресурса Рекуиредресаурцеакцесс</span><span class="sxs-lookup"><span data-stu-id="d73ca-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d73ca-106">Задает набор областей разрешений OAuth 2,0 и ролей приложения в указанном ресурсе, к которому приложение требует доступ.</span><span class="sxs-lookup"><span data-stu-id="d73ca-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="d73ca-107">Указанные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** ) при вызове приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="d73ca-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="d73ca-108">Свойство **рекуиредресаурцеакцесс** объекта [Application](application.md) представляет собой коллекцию **рекиредресаурцеакцесс**.</span><span class="sxs-lookup"><span data-stu-id="d73ca-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d73ca-109">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d73ca-109">JSON representation</span></span>

<span data-ttu-id="d73ca-110">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d73ca-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d73ca-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="d73ca-111">Properties</span></span>
| <span data-ttu-id="d73ca-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="d73ca-112">Property</span></span>     | <span data-ttu-id="d73ca-113">Тип</span><span class="sxs-lookup"><span data-stu-id="d73ca-113">Type</span></span>   |<span data-ttu-id="d73ca-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d73ca-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d73ca-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="d73ca-115">resourceAccess</span></span>|<span data-ttu-id="d73ca-116">Коллекция [ресаурцеакцесс](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="d73ca-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="d73ca-117">Список областей разрешений OAuth 2.0 и ролей приложений, которые требуются приложению из указанного ресурса.</span><span class="sxs-lookup"><span data-stu-id="d73ca-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="d73ca-118">Ресаурцеаппид</span><span class="sxs-lookup"><span data-stu-id="d73ca-118">resourceAppId</span></span>|<span data-ttu-id="d73ca-119">String</span><span class="sxs-lookup"><span data-stu-id="d73ca-119">String</span></span>|<span data-ttu-id="d73ca-120">Уникальный идентификатор ресурса, доступ к которому требуется приложению.</span><span class="sxs-lookup"><span data-stu-id="d73ca-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="d73ca-121">Он должен быть равен **AppID** , объявленному в целевом приложении ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d73ca-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
