---
title: Тип ресурса appIdentity
description: Указывает идентификатор приложения, выполнившего действия или была изменена. Включает в себя код приложения, имя, идентификатор участника-службы и имя. Этот ресурс вызывается directoryAudit API
ms.openlocfilehash: 6fcbe8dbb1e17139111c5f1fa9e8681cd1b996a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078630"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="7413f-105">Тип ресурса appIdentity</span><span class="sxs-lookup"><span data-stu-id="7413f-105">appIdentity resource type</span></span>
<span data-ttu-id="7413f-106">Указывает идентификатор приложения, выполнившего действия или была изменена.</span><span class="sxs-lookup"><span data-stu-id="7413f-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="7413f-107">Включает в себя код приложения, имя, идентификатор участника-службы и имя.</span><span class="sxs-lookup"><span data-stu-id="7413f-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="7413f-108">Этот ресурс вызывается [directoryAudit](../api/directoryaudit-get.md) API</span><span class="sxs-lookup"><span data-stu-id="7413f-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="7413f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7413f-109">Properties</span></span>
| <span data-ttu-id="7413f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7413f-110">Property</span></span>     | <span data-ttu-id="7413f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7413f-111">Type</span></span>   |<span data-ttu-id="7413f-112">Description</span><span class="sxs-lookup"><span data-stu-id="7413f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7413f-113">appId</span><span class="sxs-lookup"><span data-stu-id="7413f-113">appId</span></span>|<span data-ttu-id="7413f-114">String</span><span class="sxs-lookup"><span data-stu-id="7413f-114">String</span></span>|<span data-ttu-id="7413f-115">Указывает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7413f-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="7413f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="7413f-116">displayName</span></span>|<span data-ttu-id="7413f-117">String</span><span class="sxs-lookup"><span data-stu-id="7413f-117">String</span></span>|<span data-ttu-id="7413f-118">Ссылается на имя приложения, отображаемые на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7413f-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="7413f-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="7413f-119">servicePrincipalId</span></span>|<span data-ttu-id="7413f-120">String</span><span class="sxs-lookup"><span data-stu-id="7413f-120">String</span></span>|<span data-ttu-id="7413f-121">Указывает уникальный идентификатор GUID, указывающее идентификатор участника-службы в Azure Active Directory для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="7413f-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="7413f-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="7413f-122">servicePrincipalName</span></span>|<span data-ttu-id="7413f-123">String</span><span class="sxs-lookup"><span data-stu-id="7413f-123">String</span></span>|<span data-ttu-id="7413f-124">Ссылается на имя участника-службы — это имя приложения в клиентов.</span><span class="sxs-lookup"><span data-stu-id="7413f-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7413f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7413f-125">JSON representation</span></span>

<span data-ttu-id="7413f-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7413f-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->