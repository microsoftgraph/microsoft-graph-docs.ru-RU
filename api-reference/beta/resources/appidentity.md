---
title: Тип ресурса appIdentity
description: Указывает удостоверение приложения, которое выполнило действие или было изменено. Включает в себя ИД приложения, имя, ИД основного приложения-службы и имя. Этот ресурс вызван API directoryAudit
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: sureshja
ms.openlocfilehash: 2949acd00b3ef494d7fb3999c180631cf8609cc3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137048"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="233da-105">Тип ресурса appIdentity</span><span class="sxs-lookup"><span data-stu-id="233da-105">appIdentity resource type</span></span>

<span data-ttu-id="233da-106">Пространство имен: microsoft.graph указывает удостоверение приложения, которое выполнило действие или было изменено.</span><span class="sxs-lookup"><span data-stu-id="233da-106">Namespace: microsoft.graph Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="233da-107">Включает в себя ИД приложения, имя, ИД основного приложения-службы и имя.</span><span class="sxs-lookup"><span data-stu-id="233da-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="233da-108">Этот ресурс вызван API [directoryAudit](../api/directoryaudit-get.md)</span><span class="sxs-lookup"><span data-stu-id="233da-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="233da-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="233da-109">Properties</span></span>
| <span data-ttu-id="233da-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="233da-110">Property</span></span>     | <span data-ttu-id="233da-111">Тип</span><span class="sxs-lookup"><span data-stu-id="233da-111">Type</span></span>   |<span data-ttu-id="233da-112">Описание</span><span class="sxs-lookup"><span data-stu-id="233da-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="233da-113">appId</span><span class="sxs-lookup"><span data-stu-id="233da-113">appId</span></span>|<span data-ttu-id="233da-114">String</span><span class="sxs-lookup"><span data-stu-id="233da-114">String</span></span>|<span data-ttu-id="233da-115">Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="233da-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="233da-116">displayName</span><span class="sxs-lookup"><span data-stu-id="233da-116">displayName</span></span>|<span data-ttu-id="233da-117">Строка</span><span class="sxs-lookup"><span data-stu-id="233da-117">String</span></span>|<span data-ttu-id="233da-118">Указывает на имя приложения, отображаемую на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="233da-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="233da-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="233da-119">servicePrincipalId</span></span>|<span data-ttu-id="233da-120">Строка</span><span class="sxs-lookup"><span data-stu-id="233da-120">String</span></span>|<span data-ttu-id="233da-121">Ссылается на уникальный GUID, указывающий ИД основного службы в Azure Active Directory для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="233da-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="233da-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="233da-122">servicePrincipalName</span></span>|<span data-ttu-id="233da-123">String</span><span class="sxs-lookup"><span data-stu-id="233da-123">String</span></span>|<span data-ttu-id="233da-124">Ссылается на имя основного службы имя приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="233da-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="233da-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="233da-125">JSON representation</span></span>

<span data-ttu-id="233da-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="233da-126">Here is a JSON representation of the resource.</span></span>

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


