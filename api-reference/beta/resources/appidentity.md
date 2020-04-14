---
title: Тип ресурса Аппидентити
description: Указывает идентификатор приложения, который выполнил действие или изменился. Включает идентификатор приложения, имя, идентификатор и имя участника службы. Этот ресурс вызывается API Директоряудит
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d9d2c6ff3ceadd55404d32e57d1837c4023771f4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450170"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="37882-105">Тип ресурса Аппидентити</span><span class="sxs-lookup"><span data-stu-id="37882-105">appIdentity resource type</span></span>

<span data-ttu-id="37882-106">Пространство имен: Microsoft. Graph указывает идентификатор приложения, который выполнил действие или изменился.</span><span class="sxs-lookup"><span data-stu-id="37882-106">Namespace: microsoft.graph Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="37882-107">Включает идентификатор приложения, имя, идентификатор и имя участника службы.</span><span class="sxs-lookup"><span data-stu-id="37882-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="37882-108">Этот ресурс вызывается API [директоряудит](../api/directoryaudit-get.md)</span><span class="sxs-lookup"><span data-stu-id="37882-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="37882-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="37882-109">Properties</span></span>
| <span data-ttu-id="37882-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="37882-110">Property</span></span>     | <span data-ttu-id="37882-111">Тип</span><span class="sxs-lookup"><span data-stu-id="37882-111">Type</span></span>   |<span data-ttu-id="37882-112">Описание</span><span class="sxs-lookup"><span data-stu-id="37882-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37882-113">appId</span><span class="sxs-lookup"><span data-stu-id="37882-113">appId</span></span>|<span data-ttu-id="37882-114">String</span><span class="sxs-lookup"><span data-stu-id="37882-114">String</span></span>|<span data-ttu-id="37882-115">Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="37882-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="37882-116">displayName</span><span class="sxs-lookup"><span data-stu-id="37882-116">displayName</span></span>|<span data-ttu-id="37882-117">Строка</span><span class="sxs-lookup"><span data-stu-id="37882-117">String</span></span>|<span data-ttu-id="37882-118">Указывает на имя приложения, отображаемое на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="37882-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="37882-119">сервицепринЦипалид</span><span class="sxs-lookup"><span data-stu-id="37882-119">servicePrincipalId</span></span>|<span data-ttu-id="37882-120">String</span><span class="sxs-lookup"><span data-stu-id="37882-120">String</span></span>|<span data-ttu-id="37882-121">Указывает уникальный идентификатор GUID, указывающий идентификатор участника службы в Azure Active Directory для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="37882-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="37882-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="37882-122">servicePrincipalName</span></span>|<span data-ttu-id="37882-123">String</span><span class="sxs-lookup"><span data-stu-id="37882-123">String</span></span>|<span data-ttu-id="37882-124">— Имя участника-службы — это имя приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="37882-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37882-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37882-125">JSON representation</span></span>

<span data-ttu-id="37882-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37882-126">Here is a JSON representation of the resource.</span></span>

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
