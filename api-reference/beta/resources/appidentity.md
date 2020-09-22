---
title: Тип ресурса Аппидентити
description: Указывает идентификатор приложения, который выполнил действие или изменился. Включает идентификатор приложения, имя, идентификатор и имя участника службы. Этот ресурс вызывается API Директоряудит
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: ed814cb4e096ff8e13bdb8f06ede6cad4f94c6d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004202"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="d2354-105">Тип ресурса Аппидентити</span><span class="sxs-lookup"><span data-stu-id="d2354-105">appIdentity resource type</span></span>

<span data-ttu-id="d2354-106">Пространство имен: Microsoft. Graph указывает идентификатор приложения, который выполнил действие или изменился.</span><span class="sxs-lookup"><span data-stu-id="d2354-106">Namespace: microsoft.graph Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="d2354-107">Включает идентификатор приложения, имя, идентификатор и имя участника службы.</span><span class="sxs-lookup"><span data-stu-id="d2354-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="d2354-108">Этот ресурс вызывается API [директоряудит](../api/directoryaudit-get.md)</span><span class="sxs-lookup"><span data-stu-id="d2354-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="d2354-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2354-109">Properties</span></span>
| <span data-ttu-id="d2354-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2354-110">Property</span></span>     | <span data-ttu-id="d2354-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d2354-111">Type</span></span>   |<span data-ttu-id="d2354-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d2354-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2354-113">appId</span><span class="sxs-lookup"><span data-stu-id="d2354-113">appId</span></span>|<span data-ttu-id="d2354-114">String</span><span class="sxs-lookup"><span data-stu-id="d2354-114">String</span></span>|<span data-ttu-id="d2354-115">Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d2354-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="d2354-116">displayName</span><span class="sxs-lookup"><span data-stu-id="d2354-116">displayName</span></span>|<span data-ttu-id="d2354-117">String</span><span class="sxs-lookup"><span data-stu-id="d2354-117">String</span></span>|<span data-ttu-id="d2354-118">Указывает на имя приложения, отображаемое на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d2354-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="d2354-119">сервицепринЦипалид</span><span class="sxs-lookup"><span data-stu-id="d2354-119">servicePrincipalId</span></span>|<span data-ttu-id="d2354-120">String</span><span class="sxs-lookup"><span data-stu-id="d2354-120">String</span></span>|<span data-ttu-id="d2354-121">Указывает уникальный идентификатор GUID, указывающий идентификатор участника службы в Azure Active Directory для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="d2354-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="d2354-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="d2354-122">servicePrincipalName</span></span>|<span data-ttu-id="d2354-123">String</span><span class="sxs-lookup"><span data-stu-id="d2354-123">String</span></span>|<span data-ttu-id="d2354-124">— Имя участника-службы — это имя приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d2354-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d2354-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d2354-125">JSON representation</span></span>

<span data-ttu-id="d2354-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2354-126">Here is a JSON representation of the resource.</span></span>

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


