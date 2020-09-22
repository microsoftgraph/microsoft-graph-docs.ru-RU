---
title: Тип ресурса Аппидентити
description: Указывает идентификатор приложения, который выполнил действие или изменился. Включает идентификатор приложения, имя, идентификатор и имя участника службы. Этот ресурс вызывается API Директоряудит
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1878aa01f2a6594f102647b6642eab6f301fa91
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988599"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="5a7d6-105">Тип ресурса Аппидентити</span><span class="sxs-lookup"><span data-stu-id="5a7d6-105">appIdentity resource type</span></span>

<span data-ttu-id="5a7d6-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a7d6-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a7d6-107">Указывает идентификатор приложения, который выполнил действие или изменился.</span><span class="sxs-lookup"><span data-stu-id="5a7d6-107">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="5a7d6-108">Содержит идентификатор приложения, имя и идентификатор и имя участника службы.</span><span class="sxs-lookup"><span data-stu-id="5a7d6-108">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="5a7d6-109">Этот ресурс используется операцией [Get директоряудит](../api/directoryaudit-get.md) .</span><span class="sxs-lookup"><span data-stu-id="5a7d6-109">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="5a7d6-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a7d6-110">Properties</span></span>

| <span data-ttu-id="5a7d6-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a7d6-111">Property</span></span>     | <span data-ttu-id="5a7d6-112">Тип</span><span class="sxs-lookup"><span data-stu-id="5a7d6-112">Type</span></span>   |<span data-ttu-id="5a7d6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5a7d6-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a7d6-114">appId</span><span class="sxs-lookup"><span data-stu-id="5a7d6-114">appId</span></span>|<span data-ttu-id="5a7d6-115">String</span><span class="sxs-lookup"><span data-stu-id="5a7d6-115">String</span></span>|<span data-ttu-id="5a7d6-116">Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5a7d6-116">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="5a7d6-117">displayName</span><span class="sxs-lookup"><span data-stu-id="5a7d6-117">displayName</span></span>|<span data-ttu-id="5a7d6-118">String</span><span class="sxs-lookup"><span data-stu-id="5a7d6-118">String</span></span>|<span data-ttu-id="5a7d6-119">Указывает на имя приложения, отображаемое на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5a7d6-119">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="5a7d6-120">сервицепринЦипалид</span><span class="sxs-lookup"><span data-stu-id="5a7d6-120">servicePrincipalId</span></span>|<span data-ttu-id="5a7d6-121">String</span><span class="sxs-lookup"><span data-stu-id="5a7d6-121">String</span></span>|<span data-ttu-id="5a7d6-122">Указывает уникальный идентификатор GUID, указывающий идентификатор участника службы в Azure Active Directory для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="5a7d6-122">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="5a7d6-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="5a7d6-123">servicePrincipalName</span></span>|<span data-ttu-id="5a7d6-124">String</span><span class="sxs-lookup"><span data-stu-id="5a7d6-124">String</span></span>|<span data-ttu-id="5a7d6-125">— Имя участника-службы — это имя приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5a7d6-125">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a7d6-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a7d6-126">JSON representation</span></span>

<span data-ttu-id="5a7d6-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a7d6-127">Here is a JSON representation of the resource.</span></span>

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

