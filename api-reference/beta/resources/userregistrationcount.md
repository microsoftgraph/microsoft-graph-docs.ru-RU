---
title: Тип ресурса Усеррегистратионкаунт
description: Представляет счетчик регистраций и состояние для пользователей в клиенте.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 43f151864f7ca996602e7bd2fc42f3fa4ba743d1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489507"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="33dc0-103">Тип ресурса Усеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="33dc0-103">userRegistrationCount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33dc0-104">Представляет счетчик регистраций и состояние для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="33dc0-104">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="33dc0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="33dc0-105">Properties</span></span>

| <span data-ttu-id="33dc0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="33dc0-106">Property</span></span>     | <span data-ttu-id="33dc0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="33dc0-107">Type</span></span>        | <span data-ttu-id="33dc0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="33dc0-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="33dc0-109">Регистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="33dc0-109">registrationCount</span></span> | <span data-ttu-id="33dc0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="33dc0-110">Int64</span></span> | <span data-ttu-id="33dc0-111">Предоставляет счетчик регистраций для клиента.</span><span class="sxs-lookup"><span data-stu-id="33dc0-111">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="33dc0-112">Регистратионстатус</span><span class="sxs-lookup"><span data-stu-id="33dc0-112">registrationStatus</span></span> | <span data-ttu-id="33dc0-113">String</span><span class="sxs-lookup"><span data-stu-id="33dc0-113">String</span></span> | <span data-ttu-id="33dc0-114">Представляет состояние регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="33dc0-114">Represents the status of user registration.</span></span> <span data-ttu-id="33dc0-115">`registered`Возможные значения: `enabled`,, `capable`и. `mfaRegistered`</span><span class="sxs-lookup"><span data-stu-id="33dc0-115">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="33dc0-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33dc0-116">JSON representation</span></span>

<span data-ttu-id="33dc0-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33dc0-117">The following is a JSON representation of the resource.</span></span>

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