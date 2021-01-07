---
title: Тип ресурса applicationServicePrincipal
description: Сочетание приложения и servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 77d1d9beeab406896bda53e88e9043be0a99e8fe
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777723"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="6f2f6-103">Тип ресурса applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6f2f6-103">applicationServicePrincipal resource type</span></span>

<span data-ttu-id="6f2f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f2f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f2f6-105">При добавлении экземпляра приложения из коллекции приложений Azure AD в каталоге создаются объекты [application](../resources/application.md) и [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="6f2f6-105">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="6f2f6-106">**ApplicationServicePrincipal** представляет собой совмещение объекта **application** и **servicePrincipal.**</span><span class="sxs-lookup"><span data-stu-id="6f2f6-106">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="6f2f6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6f2f6-107">Methods</span></span>

<span data-ttu-id="6f2f6-108">Нет</span><span class="sxs-lookup"><span data-stu-id="6f2f6-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="6f2f6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f2f6-109">Properties</span></span>

| <span data-ttu-id="6f2f6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f2f6-110">Property</span></span> | <span data-ttu-id="6f2f6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6f2f6-111">Type</span></span>        | <span data-ttu-id="6f2f6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2f6-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f2f6-113">application</span><span class="sxs-lookup"><span data-stu-id="6f2f6-113">application</span></span>|[<span data-ttu-id="6f2f6-114">application</span><span class="sxs-lookup"><span data-stu-id="6f2f6-114">application</span></span>](../resources/application.md)|<span data-ttu-id="6f2f6-115">Представляет приложение, зарегистрированное в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6f2f6-115">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="6f2f6-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6f2f6-116">servicePrincipal</span></span>|[<span data-ttu-id="6f2f6-117">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6f2f6-117">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="6f2f6-118">Представляет экземпляр приложения в каталоге.</span><span class="sxs-lookup"><span data-stu-id="6f2f6-118">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f2f6-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6f2f6-119">Relationships</span></span>

<span data-ttu-id="6f2f6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6f2f6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f2f6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f2f6-121">JSON representation</span></span>

<span data-ttu-id="6f2f6-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f2f6-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
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


