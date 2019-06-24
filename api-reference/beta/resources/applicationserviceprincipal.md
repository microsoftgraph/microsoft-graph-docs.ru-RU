---
title: Тип ресурса АппликатионсервицепринЦипал
description: Сочетание приложения и servicePrincipal.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3a6d0d1017f89587f1f826c4225eefc51dc5edb
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147938"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="31cd9-103">Тип ресурса АппликатионсервицепринЦипал</span><span class="sxs-lookup"><span data-stu-id="31cd9-103">applicationServicePrincipal resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31cd9-104">При добавлении экземпляра приложения из коллекции приложений Azure AD объекты [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) создаются в каталоге.</span><span class="sxs-lookup"><span data-stu-id="31cd9-104">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="31cd9-105">**АппликатионсервицепринЦипал** представляет сцепление объекта **Application** и **servicePrincipal** .</span><span class="sxs-lookup"><span data-stu-id="31cd9-105">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="31cd9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="31cd9-106">Methods</span></span>

<span data-ttu-id="31cd9-107">Нет</span><span class="sxs-lookup"><span data-stu-id="31cd9-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="31cd9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="31cd9-108">Properties</span></span>

| <span data-ttu-id="31cd9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="31cd9-109">Property</span></span> | <span data-ttu-id="31cd9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="31cd9-110">Type</span></span>        | <span data-ttu-id="31cd9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="31cd9-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31cd9-112">application</span><span class="sxs-lookup"><span data-stu-id="31cd9-112">application</span></span>|[<span data-ttu-id="31cd9-113">application</span><span class="sxs-lookup"><span data-stu-id="31cd9-113">application</span></span>](../resources/application.md)|<span data-ttu-id="31cd9-114">Представляет приложение, зарегистрированное в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31cd9-114">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="31cd9-115">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="31cd9-115">servicePrincipal</span></span>|[<span data-ttu-id="31cd9-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="31cd9-116">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="31cd9-117">Представляет экземпляр приложения в каталоге.</span><span class="sxs-lookup"><span data-stu-id="31cd9-117">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31cd9-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="31cd9-118">Relationships</span></span>

<span data-ttu-id="31cd9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="31cd9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31cd9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31cd9-120">JSON representation</span></span>

<span data-ttu-id="31cd9-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31cd9-121">The following is a JSON representation of the resource.</span></span>

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
