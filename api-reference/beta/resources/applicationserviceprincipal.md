---
title: Тип ресурса АппликатионсервицепринЦипал
description: Сочетание приложения и servicePrincipal.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9a7cc33e05c28e5552815778e86e5b1b9e7aaf06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508284"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="6d5be-103">Тип ресурса АппликатионсервицепринЦипал</span><span class="sxs-lookup"><span data-stu-id="6d5be-103">applicationServicePrincipal resource type</span></span>

<span data-ttu-id="6d5be-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6d5be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d5be-105">При добавлении экземпляра приложения из коллекции приложений Azure AD объекты [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) создаются в каталоге.</span><span class="sxs-lookup"><span data-stu-id="6d5be-105">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="6d5be-106">**АппликатионсервицепринЦипал** представляет сцепление объекта **Application** и **servicePrincipal** .</span><span class="sxs-lookup"><span data-stu-id="6d5be-106">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="6d5be-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6d5be-107">Methods</span></span>

<span data-ttu-id="6d5be-108">Нет</span><span class="sxs-lookup"><span data-stu-id="6d5be-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="6d5be-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d5be-109">Properties</span></span>

| <span data-ttu-id="6d5be-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d5be-110">Property</span></span> | <span data-ttu-id="6d5be-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6d5be-111">Type</span></span>        | <span data-ttu-id="6d5be-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6d5be-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d5be-113">application</span><span class="sxs-lookup"><span data-stu-id="6d5be-113">application</span></span>|[<span data-ttu-id="6d5be-114">application</span><span class="sxs-lookup"><span data-stu-id="6d5be-114">application</span></span>](../resources/application.md)|<span data-ttu-id="6d5be-115">Представляет приложение, зарегистрированное в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6d5be-115">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="6d5be-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6d5be-116">servicePrincipal</span></span>|[<span data-ttu-id="6d5be-117">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6d5be-117">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="6d5be-118">Представляет экземпляр приложения в каталоге.</span><span class="sxs-lookup"><span data-stu-id="6d5be-118">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d5be-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6d5be-119">Relationships</span></span>

<span data-ttu-id="6d5be-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6d5be-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d5be-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d5be-121">JSON representation</span></span>

<span data-ttu-id="6d5be-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d5be-122">The following is a JSON representation of the resource.</span></span>

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
