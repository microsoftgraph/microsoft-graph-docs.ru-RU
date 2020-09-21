---
title: Тип ресурса АппликатионсервицепринЦипал
description: Сочетание приложения и servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b45da6cd8533d9522d42428f6e222a669f17e681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050271"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="62932-103">Тип ресурса АппликатионсервицепринЦипал</span><span class="sxs-lookup"><span data-stu-id="62932-103">applicationServicePrincipal resource type</span></span>

<span data-ttu-id="62932-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62932-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62932-105">При добавлении экземпляра приложения из коллекции приложений Azure AD объекты [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) создаются в каталоге.</span><span class="sxs-lookup"><span data-stu-id="62932-105">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="62932-106">**АппликатионсервицепринЦипал** представляет сцепление объекта **Application** и **servicePrincipal** .</span><span class="sxs-lookup"><span data-stu-id="62932-106">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="62932-107">Методы</span><span class="sxs-lookup"><span data-stu-id="62932-107">Methods</span></span>

<span data-ttu-id="62932-108">Нет</span><span class="sxs-lookup"><span data-stu-id="62932-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="62932-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="62932-109">Properties</span></span>

| <span data-ttu-id="62932-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="62932-110">Property</span></span> | <span data-ttu-id="62932-111">Тип</span><span class="sxs-lookup"><span data-stu-id="62932-111">Type</span></span>        | <span data-ttu-id="62932-112">Описание</span><span class="sxs-lookup"><span data-stu-id="62932-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62932-113">application</span><span class="sxs-lookup"><span data-stu-id="62932-113">application</span></span>|[<span data-ttu-id="62932-114">application</span><span class="sxs-lookup"><span data-stu-id="62932-114">application</span></span>](../resources/application.md)|<span data-ttu-id="62932-115">Представляет приложение, зарегистрированное в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="62932-115">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="62932-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="62932-116">servicePrincipal</span></span>|[<span data-ttu-id="62932-117">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="62932-117">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="62932-118">Представляет экземпляр приложения в каталоге.</span><span class="sxs-lookup"><span data-stu-id="62932-118">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62932-119">Связи</span><span class="sxs-lookup"><span data-stu-id="62932-119">Relationships</span></span>

<span data-ttu-id="62932-120">Нет</span><span class="sxs-lookup"><span data-stu-id="62932-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62932-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62932-121">JSON representation</span></span>

<span data-ttu-id="62932-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62932-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


