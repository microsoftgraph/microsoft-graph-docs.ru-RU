---
title: Тип ресурса appIdentity
description: Указывает идентификатор приложения, выполнившего действия или была изменена. Включает в себя код приложения, имя, идентификатор участника-службы и имя. Этот ресурс вызывается directoryAudit API
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855785"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="da700-105">Тип ресурса appIdentity</span><span class="sxs-lookup"><span data-stu-id="da700-105">appIdentity resource type</span></span>
<span data-ttu-id="da700-106">Указывает идентификатор приложения, выполнившего действия или была изменена.</span><span class="sxs-lookup"><span data-stu-id="da700-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="da700-107">Включает в себя код приложения, имя, идентификатор участника-службы и имя.</span><span class="sxs-lookup"><span data-stu-id="da700-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="da700-108">Этот ресурс вызывается [directoryAudit](../api/directoryaudit-get.md) API</span><span class="sxs-lookup"><span data-stu-id="da700-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="da700-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="da700-109">Properties</span></span>
| <span data-ttu-id="da700-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="da700-110">Property</span></span>     | <span data-ttu-id="da700-111">Тип</span><span class="sxs-lookup"><span data-stu-id="da700-111">Type</span></span>   |<span data-ttu-id="da700-112">Описание</span><span class="sxs-lookup"><span data-stu-id="da700-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da700-113">appId</span><span class="sxs-lookup"><span data-stu-id="da700-113">appId</span></span>|<span data-ttu-id="da700-114">String</span><span class="sxs-lookup"><span data-stu-id="da700-114">String</span></span>|<span data-ttu-id="da700-115">Указывает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="da700-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="da700-116">displayName</span><span class="sxs-lookup"><span data-stu-id="da700-116">displayName</span></span>|<span data-ttu-id="da700-117">Строка</span><span class="sxs-lookup"><span data-stu-id="da700-117">String</span></span>|<span data-ttu-id="da700-118">Ссылается на имя приложения, отображаемые на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="da700-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="da700-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="da700-119">servicePrincipalId</span></span>|<span data-ttu-id="da700-120">Строка</span><span class="sxs-lookup"><span data-stu-id="da700-120">String</span></span>|<span data-ttu-id="da700-121">Указывает уникальный идентификатор GUID, указывающее идентификатор участника-службы в Azure Active Directory для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="da700-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="da700-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="da700-122">servicePrincipalName</span></span>|<span data-ttu-id="da700-123">String</span><span class="sxs-lookup"><span data-stu-id="da700-123">String</span></span>|<span data-ttu-id="da700-124">Ссылается на имя участника-службы — это имя приложения в клиентов.</span><span class="sxs-lookup"><span data-stu-id="da700-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da700-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da700-125">JSON representation</span></span>

<span data-ttu-id="da700-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da700-126">Here is a JSON representation of the resource.</span></span>

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
