---
title: Тип ресурса ПровисионингсервицепринЦипал
description: Представляет участника службы, используемого для подготовки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e163be94269ee6a75f148b460f728a36e8945645
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446578"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="84167-103">Тип ресурса ПровисионингсервицепринЦипал</span><span class="sxs-lookup"><span data-stu-id="84167-103">provisioningServicePrincipal resource type</span></span>

<span data-ttu-id="84167-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84167-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84167-105">Представляет участника службы, используемого для подготовки.</span><span class="sxs-lookup"><span data-stu-id="84167-105">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="84167-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="84167-106">Properties</span></span>

| <span data-ttu-id="84167-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="84167-107">Property</span></span>     | <span data-ttu-id="84167-108">Тип</span><span class="sxs-lookup"><span data-stu-id="84167-108">Type</span></span>        | <span data-ttu-id="84167-109">Описание</span><span class="sxs-lookup"><span data-stu-id="84167-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84167-110">id</span><span class="sxs-lookup"><span data-stu-id="84167-110">id</span></span>|<span data-ttu-id="84167-111">Строка</span><span class="sxs-lookup"><span data-stu-id="84167-111">String</span></span>|<span data-ttu-id="84167-112">Уникально идентифицирует **servicePrincipal** , используемый для подготовки.</span><span class="sxs-lookup"><span data-stu-id="84167-112">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="84167-113">name</span><span class="sxs-lookup"><span data-stu-id="84167-113">name</span></span>|<span data-ttu-id="84167-114">String</span><span class="sxs-lookup"><span data-stu-id="84167-114">String</span></span>| <span data-ttu-id="84167-115">Определяемое пользователем имя для **servicePrincipal**.</span><span class="sxs-lookup"><span data-stu-id="84167-115">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84167-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84167-116">JSON representation</span></span>

<span data-ttu-id="84167-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84167-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningServicePrincipal",
  "baseType": null
}-->

```json
{
  "id": "String",
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
