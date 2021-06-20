---
title: тип ресурса servicePrincipalIdentity
description: Модели основного удостоверения службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 231a0d9dc811569de23412d6ad76a2ba35f6c58b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031369"
---
# <a name="serviceprincipalidentity-resource-type"></a><span data-ttu-id="457c6-103">тип ресурса servicePrincipalIdentity</span><span class="sxs-lookup"><span data-stu-id="457c6-103">servicePrincipalIdentity resource type</span></span>

<span data-ttu-id="457c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="457c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="457c6-105">Модели основного удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="457c6-105">Models a service principal identity.</span></span>

<span data-ttu-id="457c6-106">Наследует от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="457c6-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="457c6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="457c6-107">Properties</span></span>
|<span data-ttu-id="457c6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="457c6-108">Property</span></span>|<span data-ttu-id="457c6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="457c6-109">Type</span></span>|<span data-ttu-id="457c6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="457c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457c6-111">appId</span><span class="sxs-lookup"><span data-stu-id="457c6-111">appId</span></span>|<span data-ttu-id="457c6-112">String</span><span class="sxs-lookup"><span data-stu-id="457c6-112">String</span></span>|<span data-ttu-id="457c6-113">Идентификатор приложения для директора службы.</span><span class="sxs-lookup"><span data-stu-id="457c6-113">The application identifier of the service principal.</span></span>|
|<span data-ttu-id="457c6-114">displayName</span><span class="sxs-lookup"><span data-stu-id="457c6-114">displayName</span></span>|<span data-ttu-id="457c6-115">String</span><span class="sxs-lookup"><span data-stu-id="457c6-115">String</span></span>|<span data-ttu-id="457c6-116">Отображение имени основного удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="457c6-116">The display name of the service principal identity.</span></span> <span data-ttu-id="457c6-117">Унаследованный от [удостоверения](../resources/identity.md)</span><span class="sxs-lookup"><span data-stu-id="457c6-117">Inherited from [identity](../resources/identity.md)</span></span>|
|<span data-ttu-id="457c6-118">id</span><span class="sxs-lookup"><span data-stu-id="457c6-118">id</span></span>|<span data-ttu-id="457c6-119">String</span><span class="sxs-lookup"><span data-stu-id="457c6-119">String</span></span>|<span data-ttu-id="457c6-120">Идентификатор основного удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="457c6-120">The identifier of the service principal identity.</span></span> <span data-ttu-id="457c6-121">Унаследованный от [удостоверения](../resources/identity.md)</span><span class="sxs-lookup"><span data-stu-id="457c6-121">Inherited from [identity](../resources/identity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="457c6-122">Связи</span><span class="sxs-lookup"><span data-stu-id="457c6-122">Relationships</span></span>
<span data-ttu-id="457c6-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="457c6-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="457c6-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="457c6-124">JSON representation</span></span>
<span data-ttu-id="457c6-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="457c6-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```
