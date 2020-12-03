---
title: Тип ресурса Усеррегистратионкаунт
description: Представляет счетчик регистраций и состояние для пользователей в клиенте.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 3e3a5e7e3925f5528d5ce73a15233cea8e50eebd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524185"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="af238-103">Тип ресурса Усеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="af238-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="af238-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af238-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af238-105">Представляет счетчик регистраций и состояние для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="af238-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="af238-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="af238-106">Properties</span></span>

| <span data-ttu-id="af238-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="af238-107">Property</span></span>     | <span data-ttu-id="af238-108">Тип</span><span class="sxs-lookup"><span data-stu-id="af238-108">Type</span></span>        | <span data-ttu-id="af238-109">Описание</span><span class="sxs-lookup"><span data-stu-id="af238-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="af238-110">регистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="af238-110">registrationCount</span></span> | <span data-ttu-id="af238-111">Int64</span><span class="sxs-lookup"><span data-stu-id="af238-111">Int64</span></span> | <span data-ttu-id="af238-112">Предоставляет счетчик регистраций для клиента.</span><span class="sxs-lookup"><span data-stu-id="af238-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="af238-113">регистратионстатус</span><span class="sxs-lookup"><span data-stu-id="af238-113">registrationStatus</span></span> | <span data-ttu-id="af238-114">String</span><span class="sxs-lookup"><span data-stu-id="af238-114">String</span></span> | <span data-ttu-id="af238-115">Представляет состояние регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="af238-115">Represents the status of user registration.</span></span> <span data-ttu-id="af238-116">Возможные значения: `registered` , `enabled` , `capable` и `mfaRegistered` .</span><span class="sxs-lookup"><span data-stu-id="af238-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="af238-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af238-117">JSON representation</span></span>

<span data-ttu-id="af238-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af238-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userRegistrationCount",
  "baseType": null
}-->

```json
{ 
  "registrationStatus":"String", 
  "registrationCount": 23423
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

