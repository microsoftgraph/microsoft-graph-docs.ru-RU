---
title: Тип ресурса Аппидентити
description: Указывает идентификатор приложения, который выполнил действие или изменился. Включает идентификатор приложения, имя, идентификатор и имя участника службы. Этот ресурс вызывается API Директоряудит
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a8b2c9185f595bf4ab534dda5a73b1a5f40fd17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030095"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="81940-105">Тип ресурса Аппидентити</span><span class="sxs-lookup"><span data-stu-id="81940-105">appIdentity resource type</span></span>

<span data-ttu-id="81940-106">Указывает идентификатор приложения, который выполнил действие или изменился.</span><span class="sxs-lookup"><span data-stu-id="81940-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="81940-107">Содержит идентификатор приложения, имя и идентификатор и имя участника службы.</span><span class="sxs-lookup"><span data-stu-id="81940-107">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="81940-108">Этот ресурс используется операцией [Get директоряудит](../api/directoryaudit-get.md) .</span><span class="sxs-lookup"><span data-stu-id="81940-108">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="81940-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="81940-109">Properties</span></span>

| <span data-ttu-id="81940-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="81940-110">Property</span></span>     | <span data-ttu-id="81940-111">Тип</span><span class="sxs-lookup"><span data-stu-id="81940-111">Type</span></span>   |<span data-ttu-id="81940-112">Описание</span><span class="sxs-lookup"><span data-stu-id="81940-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81940-113">appId</span><span class="sxs-lookup"><span data-stu-id="81940-113">appId</span></span>|<span data-ttu-id="81940-114">String</span><span class="sxs-lookup"><span data-stu-id="81940-114">String</span></span>|<span data-ttu-id="81940-115">Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="81940-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="81940-116">displayName</span><span class="sxs-lookup"><span data-stu-id="81940-116">displayName</span></span>|<span data-ttu-id="81940-117">Строка</span><span class="sxs-lookup"><span data-stu-id="81940-117">String</span></span>|<span data-ttu-id="81940-118">Указывает на имя приложения, отображаемое на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="81940-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="81940-119">СервицепринЦипалид</span><span class="sxs-lookup"><span data-stu-id="81940-119">servicePrincipalId</span></span>|<span data-ttu-id="81940-120">String</span><span class="sxs-lookup"><span data-stu-id="81940-120">String</span></span>|<span data-ttu-id="81940-121">Указывает уникальный идентификатор GUID, указывающий идентификатор участника службы в Azure Active Directory для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="81940-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="81940-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="81940-122">servicePrincipalName</span></span>|<span data-ttu-id="81940-123">String</span><span class="sxs-lookup"><span data-stu-id="81940-123">String</span></span>|<span data-ttu-id="81940-124">— Имя участника-службы — это имя приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="81940-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81940-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81940-125">JSON representation</span></span>

<span data-ttu-id="81940-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81940-126">Here is a JSON representation of the resource.</span></span>

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
